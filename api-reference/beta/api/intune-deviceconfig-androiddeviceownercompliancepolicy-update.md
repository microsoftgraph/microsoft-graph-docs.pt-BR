---
title: Atualizar androidDeviceOwnerCompliancePolicy
description: Atualiza as propriedades de um objeto androidDeviceOwnerCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1895002b73e33bad59e13de870b9d965f1e9ce5d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933218"
---
# <a name="update-androiddeviceownercompliancepolicy"></a><span data-ttu-id="cbe5e-103">Atualizar androidDeviceOwnerCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="cbe5e-103">Update androidDeviceOwnerCompliancePolicy</span></span>

> <span data-ttu-id="cbe5e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbe5e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbe5e-106">Atualiza as propriedades de um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cbe5e-106">Update the properties of a [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbe5e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbe5e-107">Prerequisites</span></span>
<span data-ttu-id="cbe5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbe5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbe5e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbe5e-110">Permission type</span></span>|<span data-ttu-id="cbe5e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbe5e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbe5e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbe5e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cbe5e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbe5e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-115">Not supported.</span></span>|
|<span data-ttu-id="cbe5e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbe5e-116">Application</span></span>|<span data-ttu-id="cbe5e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbe5e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbe5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="cbe5e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbe5e-119">Request headers</span></span>
|<span data-ttu-id="cbe5e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbe5e-120">Header</span></span>|<span data-ttu-id="cbe5e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cbe5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbe5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbe5e-122">Authorization</span></span>|<span data-ttu-id="cbe5e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbe5e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbe5e-124">Accept</span></span>|<span data-ttu-id="cbe5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbe5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbe5e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbe5e-126">Request body</span></span>
<span data-ttu-id="cbe5e-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="cbe5e-127">In the request body, supply a JSON representation for the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object.</span></span>

<span data-ttu-id="cbe5e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cbe5e-128">The following table shows the properties that are required when you create the [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md).</span></span>

|<span data-ttu-id="cbe5e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbe5e-129">Property</span></span>|<span data-ttu-id="cbe5e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbe5e-130">Type</span></span>|<span data-ttu-id="cbe5e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbe5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbe5e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cbe5e-132">roleScopeTagIds</span></span>|<span data-ttu-id="cbe5e-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbe5e-133">String collection</span></span>|<span data-ttu-id="cbe5e-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cbe5e-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-136">id</span><span class="sxs-lookup"><span data-stu-id="cbe5e-136">id</span></span>|<span data-ttu-id="cbe5e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbe5e-137">String</span></span>|<span data-ttu-id="cbe5e-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-138">Key of the entity.</span></span> <span data-ttu-id="cbe5e-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbe5e-140">createdDateTime</span></span>|<span data-ttu-id="cbe5e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbe5e-141">DateTimeOffset</span></span>|<span data-ttu-id="cbe5e-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-142">DateTime the object was created.</span></span> <span data-ttu-id="cbe5e-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-144">description</span><span class="sxs-lookup"><span data-stu-id="cbe5e-144">description</span></span>|<span data-ttu-id="cbe5e-145">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-145">String</span></span>|<span data-ttu-id="cbe5e-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cbe5e-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbe5e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cbe5e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbe5e-149">DateTimeOffset</span></span>|<span data-ttu-id="cbe5e-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="cbe5e-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="cbe5e-152">displayName</span></span>|<span data-ttu-id="cbe5e-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbe5e-153">String</span></span>|<span data-ttu-id="cbe5e-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cbe5e-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-156">version</span><span class="sxs-lookup"><span data-stu-id="cbe5e-156">version</span></span>|<span data-ttu-id="cbe5e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-157">Int32</span></span>|<span data-ttu-id="cbe5e-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-158">Version of the device configuration.</span></span> <span data-ttu-id="cbe5e-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cbe5e-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="cbe5e-160">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="cbe5e-160">osMinimumVersion</span></span>|<span data-ttu-id="cbe5e-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbe5e-161">String</span></span>|<span data-ttu-id="cbe5e-162">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-162">Minimum Android version.</span></span>|
|<span data-ttu-id="cbe5e-163">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="cbe5e-163">osMaximumVersion</span></span>|<span data-ttu-id="cbe5e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbe5e-164">String</span></span>|<span data-ttu-id="cbe5e-165">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-165">Maximum Android version.</span></span>|
|<span data-ttu-id="cbe5e-166">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="cbe5e-166">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="cbe5e-167">String</span><span class="sxs-lookup"><span data-stu-id="cbe5e-167">String</span></span>|<span data-ttu-id="cbe5e-168">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-168">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="cbe5e-169">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cbe5e-169">passwordRequired</span></span>|<span data-ttu-id="cbe5e-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="cbe5e-170">Boolean</span></span>|<span data-ttu-id="cbe5e-171">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-171">Require a password to unlock device.</span></span>|
|<span data-ttu-id="cbe5e-172">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cbe5e-172">passwordMinimumLength</span></span>|<span data-ttu-id="cbe5e-173">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-173">Int32</span></span>|<span data-ttu-id="cbe5e-174">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-174">Minimum password length.</span></span> <span data-ttu-id="cbe5e-175">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-175">Valid values 4 to 16</span></span>|
|<span data-ttu-id="cbe5e-176">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-176">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="cbe5e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-177">Int32</span></span>|<span data-ttu-id="cbe5e-178">Indica o número mínimo de caracteres de letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-178">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="cbe5e-179">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-180">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-180">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="cbe5e-181">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-181">Int32</span></span>|<span data-ttu-id="cbe5e-182">Indica o número mínimo de caracteres de maiúsculas e minúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-182">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="cbe5e-183">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-183">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-184">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-184">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="cbe5e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-185">Int32</span></span>|<span data-ttu-id="cbe5e-186">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-186">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="cbe5e-187">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-187">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-188">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-188">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="cbe5e-189">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-189">Int32</span></span>|<span data-ttu-id="cbe5e-190">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-190">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="cbe5e-191">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-192">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-192">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="cbe5e-193">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-193">Int32</span></span>|<span data-ttu-id="cbe5e-194">Indica o número mínimo de caracteres de símbolo necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-194">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="cbe5e-195">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-195">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-196">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="cbe5e-196">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="cbe5e-197">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-197">Int32</span></span>|<span data-ttu-id="cbe5e-198">Indica o número mínimo de caracteres de letras maiúsculas necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-198">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="cbe5e-199">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="cbe5e-199">Valid values 1 to 16</span></span>|
|<span data-ttu-id="cbe5e-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cbe5e-200">passwordRequiredType</span></span>|[<span data-ttu-id="cbe5e-201">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cbe5e-201">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="cbe5e-202">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-202">Type of characters in password.</span></span> <span data-ttu-id="cbe5e-203">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-203">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`.</span></span>|
|<span data-ttu-id="cbe5e-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cbe5e-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cbe5e-205">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-205">Int32</span></span>|<span data-ttu-id="cbe5e-206">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-206">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="cbe5e-207">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cbe5e-207">passwordExpirationDays</span></span>|<span data-ttu-id="cbe5e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-208">Int32</span></span>|<span data-ttu-id="cbe5e-209">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-209">Number of days before the password expires.</span></span> <span data-ttu-id="cbe5e-210">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="cbe5e-210">Valid values 1 to 365</span></span>|
|<span data-ttu-id="cbe5e-211">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="cbe5e-211">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="cbe5e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="cbe5e-212">Int32</span></span>|<span data-ttu-id="cbe5e-213">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-213">Number of previous passwords to block.</span></span> <span data-ttu-id="cbe5e-214">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="cbe5e-214">Valid values 1 to 24</span></span>|
|<span data-ttu-id="cbe5e-215">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="cbe5e-215">storageRequireEncryption</span></span>|<span data-ttu-id="cbe5e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbe5e-216">Boolean</span></span>|<span data-ttu-id="cbe5e-217">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-217">Require encryption on Android devices.</span></span>|



## <a name="response"></a><span data-ttu-id="cbe5e-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbe5e-218">Response</span></span>
<span data-ttu-id="cbe5e-219">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-219">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbe5e-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbe5e-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbe5e-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbe5e-221">Request</span></span>
<span data-ttu-id="cbe5e-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
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

### <a name="response"></a><span data-ttu-id="cbe5e-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbe5e-223">Response</span></span>
<span data-ttu-id="cbe5e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbe5e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




