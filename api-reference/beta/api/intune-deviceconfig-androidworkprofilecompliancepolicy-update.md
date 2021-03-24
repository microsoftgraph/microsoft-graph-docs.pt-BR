---
title: Atualizar androidWorkProfileCompliancePolicy
description: Atualize as propriedades de um objeto androidWorkProfileCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c518b0d8fadae66f894e413cf6835f216fc5664e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128289"
---
# <a name="update-androidworkprofilecompliancepolicy"></a><span data-ttu-id="ebd1b-103">Atualizar androidWorkProfileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ebd1b-103">Update androidWorkProfileCompliancePolicy</span></span>

<span data-ttu-id="ebd1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebd1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebd1b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebd1b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd1b-107">Atualize as propriedades de um [objeto androidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-107">Update the properties of a [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebd1b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebd1b-108">Prerequisites</span></span>
<span data-ttu-id="ebd1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebd1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebd1b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebd1b-111">Permission type</span></span>|<span data-ttu-id="ebd1b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebd1b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebd1b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd1b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebd1b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebd1b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-116">Not supported.</span></span>|
|<span data-ttu-id="ebd1b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebd1b-117">Application</span></span>|<span data-ttu-id="ebd1b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd1b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebd1b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="ebd1b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd1b-120">Request headers</span></span>
|<span data-ttu-id="ebd1b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebd1b-121">Header</span></span>|<span data-ttu-id="ebd1b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ebd1b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebd1b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebd1b-123">Authorization</span></span>|<span data-ttu-id="ebd1b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebd1b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebd1b-125">Accept</span></span>|<span data-ttu-id="ebd1b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebd1b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebd1b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd1b-127">Request body</span></span>
<span data-ttu-id="ebd1b-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWorkProfileCompliancePolicy.](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-128">In the request body, supply a JSON representation for the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="ebd1b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ebd1b-129">The following table shows the properties that are required when you create the [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md).</span></span>

|<span data-ttu-id="ebd1b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebd1b-130">Property</span></span>|<span data-ttu-id="ebd1b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebd1b-131">Type</span></span>|<span data-ttu-id="ebd1b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebd1b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd1b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ebd1b-133">roleScopeTagIds</span></span>|<span data-ttu-id="ebd1b-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebd1b-134">String collection</span></span>|<span data-ttu-id="ebd1b-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ebd1b-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-137">id</span><span class="sxs-lookup"><span data-stu-id="ebd1b-137">id</span></span>|<span data-ttu-id="ebd1b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebd1b-138">String</span></span>|<span data-ttu-id="ebd1b-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-139">Key of the entity.</span></span> <span data-ttu-id="ebd1b-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebd1b-141">createdDateTime</span></span>|<span data-ttu-id="ebd1b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebd1b-142">DateTimeOffset</span></span>|<span data-ttu-id="ebd1b-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-143">DateTime the object was created.</span></span> <span data-ttu-id="ebd1b-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-145">descrição</span><span class="sxs-lookup"><span data-stu-id="ebd1b-145">description</span></span>|<span data-ttu-id="ebd1b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebd1b-146">String</span></span>|<span data-ttu-id="ebd1b-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ebd1b-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebd1b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ebd1b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebd1b-150">DateTimeOffset</span></span>|<span data-ttu-id="ebd1b-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="ebd1b-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="ebd1b-153">displayName</span></span>|<span data-ttu-id="ebd1b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebd1b-154">String</span></span>|<span data-ttu-id="ebd1b-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ebd1b-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-157">version</span><span class="sxs-lookup"><span data-stu-id="ebd1b-157">version</span></span>|<span data-ttu-id="ebd1b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-158">Int32</span></span>|<span data-ttu-id="ebd1b-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-159">Version of the device configuration.</span></span> <span data-ttu-id="ebd1b-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ebd1b-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="ebd1b-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="ebd1b-161">passwordRequired</span></span>|<span data-ttu-id="ebd1b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-162">Boolean</span></span>|<span data-ttu-id="ebd1b-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="ebd1b-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ebd1b-164">passwordMinimumLength</span></span>|<span data-ttu-id="ebd1b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-165">Int32</span></span>|<span data-ttu-id="ebd1b-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-166">Minimum password length.</span></span> <span data-ttu-id="ebd1b-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="ebd1b-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="ebd1b-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ebd1b-168">passwordRequiredType</span></span>|[<span data-ttu-id="ebd1b-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ebd1b-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="ebd1b-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-170">Type of characters in password.</span></span> <span data-ttu-id="ebd1b-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="ebd1b-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ebd1b-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ebd1b-173">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-173">Int32</span></span>|<span data-ttu-id="ebd1b-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="ebd1b-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ebd1b-175">passwordExpirationDays</span></span>|<span data-ttu-id="ebd1b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-176">Int32</span></span>|<span data-ttu-id="ebd1b-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-177">Number of days before the password expires.</span></span> <span data-ttu-id="ebd1b-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="ebd1b-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="ebd1b-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ebd1b-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ebd1b-180">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-180">Int32</span></span>|<span data-ttu-id="ebd1b-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-181">Number of previous passwords to block.</span></span> <span data-ttu-id="ebd1b-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ebd1b-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ebd1b-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ebd1b-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ebd1b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ebd1b-184">Int32</span></span>|<span data-ttu-id="ebd1b-185">Número de falhas de login permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="ebd1b-186">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="ebd1b-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="ebd1b-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="ebd1b-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="ebd1b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-188">Boolean</span></span>|<span data-ttu-id="ebd1b-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="ebd1b-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="ebd1b-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="ebd1b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-191">Boolean</span></span>|<span data-ttu-id="ebd1b-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="ebd1b-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="ebd1b-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="ebd1b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-194">Boolean</span></span>|<span data-ttu-id="ebd1b-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="ebd1b-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="ebd1b-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="ebd1b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-197">Boolean</span></span>|<span data-ttu-id="ebd1b-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="ebd1b-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ebd1b-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ebd1b-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ebd1b-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ebd1b-201">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ebd1b-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ebd1b-203">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ebd1b-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="ebd1b-204">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="ebd1b-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="ebd1b-205">O MDATP exige nível mínimo de risco da Proteção Contra Ameaças Móveis para relatar o não-atendimento.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="ebd1b-206">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="ebd1b-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="ebd1b-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="ebd1b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-208">Boolean</span></span>|<span data-ttu-id="ebd1b-209">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="ebd1b-210">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ebd1b-210">osMinimumVersion</span></span>|<span data-ttu-id="ebd1b-211">String</span><span class="sxs-lookup"><span data-stu-id="ebd1b-211">String</span></span>|<span data-ttu-id="ebd1b-212">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-212">Minimum Android version.</span></span>|
|<span data-ttu-id="ebd1b-213">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ebd1b-213">osMaximumVersion</span></span>|<span data-ttu-id="ebd1b-214">String</span><span class="sxs-lookup"><span data-stu-id="ebd1b-214">String</span></span>|<span data-ttu-id="ebd1b-215">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-215">Maximum Android version.</span></span>|
|<span data-ttu-id="ebd1b-216">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="ebd1b-216">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="ebd1b-217">String</span><span class="sxs-lookup"><span data-stu-id="ebd1b-217">String</span></span>|<span data-ttu-id="ebd1b-218">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-218">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="ebd1b-219">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="ebd1b-219">storageRequireEncryption</span></span>|<span data-ttu-id="ebd1b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-220">Boolean</span></span>|<span data-ttu-id="ebd1b-221">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-221">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="ebd1b-222">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="ebd1b-222">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="ebd1b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-223">Boolean</span></span>|<span data-ttu-id="ebd1b-224">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-224">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="ebd1b-225">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="ebd1b-225">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="ebd1b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-226">Boolean</span></span>|<span data-ttu-id="ebd1b-227">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-227">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="ebd1b-228">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="ebd1b-228">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="ebd1b-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-229">Boolean</span></span>|<span data-ttu-id="ebd1b-230">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-230">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="ebd1b-231">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="ebd1b-231">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="ebd1b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-232">Boolean</span></span>|<span data-ttu-id="ebd1b-233">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-233">Require the device to have up to date security providers.</span></span> <span data-ttu-id="ebd1b-234">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-234">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="ebd1b-235">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="ebd1b-235">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="ebd1b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd1b-236">Boolean</span></span>|<span data-ttu-id="ebd1b-237">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-237">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="ebd1b-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd1b-238">Response</span></span>
<span data-ttu-id="ebd1b-239">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-239">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCompliancePolicy](../resources/intune-deviceconfig-androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebd1b-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebd1b-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebd1b-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd1b-241">Request</span></span>
<span data-ttu-id="ebd1b-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1350

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="ebd1b-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd1b-243">Response</span></span>
<span data-ttu-id="ebd1b-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebd1b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1522

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```




