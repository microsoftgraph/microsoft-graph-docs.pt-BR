---
title: Atualizar macOSCompliancePolicy
description: Atualiza as propriedades de um objeto macOSCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 922b63ba99ae17505e36a861c6d12a4b6a195c8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549857"
---
# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="afacf-103">Atualizar macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="afacf-103">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="afacf-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afacf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afacf-105">Atualiza as propriedades de um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afacf-105">Update the properties of a [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afacf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afacf-106">Prerequisites</span></span>
<span data-ttu-id="afacf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afacf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afacf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afacf-109">Permission type</span></span>|<span data-ttu-id="afacf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afacf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afacf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afacf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="afacf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afacf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afacf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afacf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afacf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afacf-114">Not supported.</span></span>|
|<span data-ttu-id="afacf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afacf-115">Application</span></span>|<span data-ttu-id="afacf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afacf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afacf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afacf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="afacf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afacf-118">Request headers</span></span>
|<span data-ttu-id="afacf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afacf-119">Header</span></span>|<span data-ttu-id="afacf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="afacf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afacf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="afacf-121">Authorization</span></span>|<span data-ttu-id="afacf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afacf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afacf-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afacf-123">Accept</span></span>|<span data-ttu-id="afacf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="afacf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afacf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afacf-125">Request body</span></span>
<span data-ttu-id="afacf-126">No corpo da solicitação, forneça uma representação JSON do objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afacf-126">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="afacf-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="afacf-127">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="afacf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afacf-128">Property</span></span>|<span data-ttu-id="afacf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="afacf-129">Type</span></span>|<span data-ttu-id="afacf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="afacf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afacf-131">id</span><span class="sxs-lookup"><span data-stu-id="afacf-131">id</span></span>|<span data-ttu-id="afacf-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afacf-132">String</span></span>|<span data-ttu-id="afacf-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afacf-133">Key of the entity.</span></span> <span data-ttu-id="afacf-134">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afacf-135">createdDateTime</span></span>|<span data-ttu-id="afacf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afacf-136">DateTimeOffset</span></span>|<span data-ttu-id="afacf-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="afacf-137">DateTime the object was created.</span></span> <span data-ttu-id="afacf-138">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-139">description</span><span class="sxs-lookup"><span data-stu-id="afacf-139">description</span></span>|<span data-ttu-id="afacf-140">String</span><span class="sxs-lookup"><span data-stu-id="afacf-140">String</span></span>|<span data-ttu-id="afacf-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afacf-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="afacf-142">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afacf-143">lastModifiedDateTime</span></span>|<span data-ttu-id="afacf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afacf-144">DateTimeOffset</span></span>|<span data-ttu-id="afacf-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="afacf-145">DateTime the object was last modified.</span></span> <span data-ttu-id="afacf-146">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="afacf-147">displayName</span></span>|<span data-ttu-id="afacf-148">String</span><span class="sxs-lookup"><span data-stu-id="afacf-148">String</span></span>|<span data-ttu-id="afacf-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afacf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="afacf-150">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-151">version</span><span class="sxs-lookup"><span data-stu-id="afacf-151">version</span></span>|<span data-ttu-id="afacf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-152">Int32</span></span>|<span data-ttu-id="afacf-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afacf-153">Version of the device configuration.</span></span> <span data-ttu-id="afacf-154">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="afacf-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="afacf-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="afacf-155">passwordRequired</span></span>|<span data-ttu-id="afacf-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="afacf-156">Boolean</span></span>|<span data-ttu-id="afacf-157">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="afacf-157">Whether or not to require a password.</span></span>|
|<span data-ttu-id="afacf-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="afacf-158">passwordBlockSimple</span></span>|<span data-ttu-id="afacf-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="afacf-159">Boolean</span></span>|<span data-ttu-id="afacf-160">Indica se senhas simples devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="afacf-160">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="afacf-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="afacf-161">passwordExpirationDays</span></span>|<span data-ttu-id="afacf-162">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-162">Int32</span></span>|<span data-ttu-id="afacf-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="afacf-163">Number of days before the password expires.</span></span> <span data-ttu-id="afacf-164">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="afacf-164">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="afacf-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="afacf-165">passwordMinimumLength</span></span>|<span data-ttu-id="afacf-166">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-166">Int32</span></span>|<span data-ttu-id="afacf-167">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="afacf-167">Minimum length of password.</span></span> <span data-ttu-id="afacf-168">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="afacf-168">Valid values 4 to 14</span></span>|
|<span data-ttu-id="afacf-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="afacf-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="afacf-170">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-170">Int32</span></span>|<span data-ttu-id="afacf-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="afacf-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="afacf-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="afacf-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="afacf-173">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-173">Int32</span></span>|<span data-ttu-id="afacf-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="afacf-174">Number of previous passwords to block.</span></span> <span data-ttu-id="afacf-175">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="afacf-175">Valid values 1 to 24</span></span>|
|<span data-ttu-id="afacf-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="afacf-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="afacf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="afacf-177">Int32</span></span>|<span data-ttu-id="afacf-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="afacf-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="afacf-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="afacf-179">passwordRequiredType</span></span>|[<span data-ttu-id="afacf-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="afacf-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="afacf-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="afacf-181">The required password type.</span></span> <span data-ttu-id="afacf-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="afacf-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="afacf-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="afacf-183">osMinimumVersion</span></span>|<span data-ttu-id="afacf-184">String</span><span class="sxs-lookup"><span data-stu-id="afacf-184">String</span></span>|<span data-ttu-id="afacf-185">Versão mínima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="afacf-185">Minimum MacOS version.</span></span>|
|<span data-ttu-id="afacf-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="afacf-186">osMaximumVersion</span></span>|<span data-ttu-id="afacf-187">String</span><span class="sxs-lookup"><span data-stu-id="afacf-187">String</span></span>|<span data-ttu-id="afacf-188">Versão máxima do MacOS.</span><span class="sxs-lookup"><span data-stu-id="afacf-188">Maximum MacOS version.</span></span>|
|<span data-ttu-id="afacf-189">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="afacf-189">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="afacf-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-190">Boolean</span></span>|<span data-ttu-id="afacf-191">Exige que dispositivos tenham habilitado a proteção de integridade do sistema.</span><span class="sxs-lookup"><span data-stu-id="afacf-191">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="afacf-192">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="afacf-192">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="afacf-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-193">Boolean</span></span>|<span data-ttu-id="afacf-194">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="afacf-194">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="afacf-195">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="afacf-195">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="afacf-196">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="afacf-196">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="afacf-197">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="afacf-197">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="afacf-198">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="afacf-198">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="afacf-199">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="afacf-199">storageRequireEncryption</span></span>|<span data-ttu-id="afacf-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-200">Boolean</span></span>|<span data-ttu-id="afacf-201">Exige criptografia em dispositivos Mac OS.</span><span class="sxs-lookup"><span data-stu-id="afacf-201">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="afacf-202">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="afacf-202">firewallEnabled</span></span>|<span data-ttu-id="afacf-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-203">Boolean</span></span>|<span data-ttu-id="afacf-204">Se o firewall deve ser habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="afacf-204">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="afacf-205">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="afacf-205">firewallBlockAllIncoming</span></span>|<span data-ttu-id="afacf-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-206">Boolean</span></span>|<span data-ttu-id="afacf-207">Corresponde à opção "bloquear todas as conexões de entrada".</span><span class="sxs-lookup"><span data-stu-id="afacf-207">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="afacf-208">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="afacf-208">firewallEnableStealthMode</span></span>|<span data-ttu-id="afacf-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="afacf-209">Boolean</span></span>|<span data-ttu-id="afacf-210">Corresponde a "Habilitar modo oculto".</span><span class="sxs-lookup"><span data-stu-id="afacf-210">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="afacf-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="afacf-211">Response</span></span>
<span data-ttu-id="afacf-212">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afacf-212">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afacf-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afacf-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="afacf-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afacf-214">Request</span></span>
<span data-ttu-id="afacf-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afacf-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afacf-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="afacf-216">Response</span></span>
<span data-ttu-id="afacf-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afacf-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



