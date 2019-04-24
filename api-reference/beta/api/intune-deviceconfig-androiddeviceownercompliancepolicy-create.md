---
title: Criar androidDeviceOwnerCompliancePolicy
description: Criar um novo objeto androidDeviceOwnerCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19ccb8cc7d778f62528b1558d762a7a938b12645
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32481203"
---
# <a name="create-androiddeviceownercompliancepolicy"></a><span data-ttu-id="87819-103">Criar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="87819-103">Create androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="87819-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87819-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87819-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87819-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87819-106">Criar um novo objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="87819-106">Create a new [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87819-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87819-107">Prerequisites</span></span>
<span data-ttu-id="87819-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87819-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87819-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87819-110">Permission type</span></span>|<span data-ttu-id="87819-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87819-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87819-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87819-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87819-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87819-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87819-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87819-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87819-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87819-115">Not supported.</span></span>|
|<span data-ttu-id="87819-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87819-116">Application</span></span>|<span data-ttu-id="87819-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87819-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87819-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87819-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="87819-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87819-119">Request headers</span></span>
|<span data-ttu-id="87819-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87819-120">Header</span></span>|<span data-ttu-id="87819-121">Valor</span><span class="sxs-lookup"><span data-stu-id="87819-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87819-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="87819-122">Authorization</span></span>|<span data-ttu-id="87819-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87819-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87819-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87819-124">Accept</span></span>|<span data-ttu-id="87819-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87819-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87819-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87819-126">Request body</span></span>
<span data-ttu-id="87819-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="87819-127">In the request body, supply a JSON representation for the androidDeviceOwnerCompliancePolicy object.</span></span>

<span data-ttu-id="87819-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="87819-128">The following table shows the properties that are required when you create the androidDeviceOwnerCompliancePolicy.</span></span>

|<span data-ttu-id="87819-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87819-129">Property</span></span>|<span data-ttu-id="87819-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="87819-130">Type</span></span>|<span data-ttu-id="87819-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="87819-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87819-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87819-132">roleScopeTagIds</span></span>|<span data-ttu-id="87819-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="87819-133">String collection</span></span>|<span data-ttu-id="87819-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="87819-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87819-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-136">id</span><span class="sxs-lookup"><span data-stu-id="87819-136">id</span></span>|<span data-ttu-id="87819-137">String</span><span class="sxs-lookup"><span data-stu-id="87819-137">String</span></span>|<span data-ttu-id="87819-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87819-138">Key of the entity.</span></span> <span data-ttu-id="87819-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87819-140">createdDateTime</span></span>|<span data-ttu-id="87819-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87819-141">DateTimeOffset</span></span>|<span data-ttu-id="87819-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="87819-142">DateTime the object was created.</span></span> <span data-ttu-id="87819-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-144">description</span><span class="sxs-lookup"><span data-stu-id="87819-144">description</span></span>|<span data-ttu-id="87819-145">String</span><span class="sxs-lookup"><span data-stu-id="87819-145">String</span></span>|<span data-ttu-id="87819-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87819-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87819-148">lastModifiedDateTime</span></span>|<span data-ttu-id="87819-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87819-149">DateTimeOffset</span></span>|<span data-ttu-id="87819-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="87819-150">DateTime the object was last modified.</span></span> <span data-ttu-id="87819-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-152">displayName</span><span class="sxs-lookup"><span data-stu-id="87819-152">displayName</span></span>|<span data-ttu-id="87819-153">String</span><span class="sxs-lookup"><span data-stu-id="87819-153">String</span></span>|<span data-ttu-id="87819-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87819-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-156">version</span><span class="sxs-lookup"><span data-stu-id="87819-156">version</span></span>|<span data-ttu-id="87819-157">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-157">Int32</span></span>|<span data-ttu-id="87819-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-158">Version of the device configuration.</span></span> <span data-ttu-id="87819-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87819-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="87819-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="87819-160">osMinimumVersion</span></span>|<span data-ttu-id="87819-161">String</span><span class="sxs-lookup"><span data-stu-id="87819-161">String</span></span>|<span data-ttu-id="87819-162">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="87819-162">Minimum Android version.</span></span>|
|<span data-ttu-id="87819-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="87819-163">osMaximumVersion</span></span>|<span data-ttu-id="87819-164">String</span><span class="sxs-lookup"><span data-stu-id="87819-164">String</span></span>|<span data-ttu-id="87819-165">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="87819-165">Maximum Android version.</span></span>|
|<span data-ttu-id="87819-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="87819-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="87819-167">String</span><span class="sxs-lookup"><span data-stu-id="87819-167">String</span></span>|<span data-ttu-id="87819-168">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="87819-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="87819-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="87819-169">passwordRequired</span></span>|<span data-ttu-id="87819-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="87819-170">Boolean</span></span>|<span data-ttu-id="87819-171">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="87819-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="87819-172">passwordMinimumLength</span></span>|<span data-ttu-id="87819-173">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-173">Int32</span></span>|<span data-ttu-id="87819-174">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="87819-174">Minimum password length.</span></span> <span data-ttu-id="87819-175">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="87819-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="87819-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-177">Int32</span></span>|<span data-ttu-id="87819-178">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="87819-179">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="87819-181">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-181">Int32</span></span>|<span data-ttu-id="87819-182">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="87819-183">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="87819-185">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-185">Int32</span></span>|<span data-ttu-id="87819-186">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="87819-187">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-188">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="87819-189">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-189">Int32</span></span>|<span data-ttu-id="87819-190">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="87819-191">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-192">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="87819-193">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-193">Int32</span></span>|<span data-ttu-id="87819-194">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="87819-195">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="87819-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="87819-197">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-197">Int32</span></span>|<span data-ttu-id="87819-198">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87819-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="87819-199">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="87819-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="87819-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="87819-200">passwordRequiredType</span></span>|[<span data-ttu-id="87819-201">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="87819-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="87819-202">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="87819-202">Type of characters in password.</span></span> <span data-ttu-id="87819-203">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="87819-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="87819-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="87819-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="87819-205">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-205">Int32</span></span>|<span data-ttu-id="87819-206">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="87819-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="87819-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="87819-207">passwordExpirationDays</span></span>|<span data-ttu-id="87819-208">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-208">Int32</span></span>|<span data-ttu-id="87819-209">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="87819-209">Number of days before the password expires.</span></span> <span data-ttu-id="87819-210">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="87819-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="87819-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="87819-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="87819-212">Int32</span><span class="sxs-lookup"><span data-stu-id="87819-212">Int32</span></span>|<span data-ttu-id="87819-213">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="87819-213">Number of previous passwords to block.</span></span> <span data-ttu-id="87819-214">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="87819-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="87819-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="87819-215">storageRequireEncryption</span></span>|<span data-ttu-id="87819-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="87819-216">Boolean</span></span>|<span data-ttu-id="87819-217">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="87819-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="87819-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="87819-218">Response</span></span>
<span data-ttu-id="87819-219">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87819-219">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87819-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87819-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="87819-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87819-221">Request</span></span>
<span data-ttu-id="87819-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87819-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 932

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="87819-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="87819-223">Response</span></span>
<span data-ttu-id="87819-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87819-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1104

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true
}
```





