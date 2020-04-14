---
title: Atualizar androidCompliancePolicy
description: Atualizar as propriedades de um objeto androidCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7a807ff101a380b74aeff1ea7fed1fc1f699b42d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43352548"
---
# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="b1395-103">Atualizar androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b1395-103">Update androidCompliancePolicy</span></span>

<span data-ttu-id="b1395-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1395-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1395-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1395-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1395-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1395-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1395-107">Atualizar as propriedades de um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1395-107">Update the properties of a [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1395-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1395-108">Prerequisites</span></span>
<span data-ttu-id="b1395-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1395-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1395-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1395-111">Permission type</span></span>|<span data-ttu-id="b1395-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1395-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1395-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1395-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1395-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1395-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1395-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1395-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1395-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1395-116">Not supported.</span></span>|
|<span data-ttu-id="b1395-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1395-117">Application</span></span>|<span data-ttu-id="b1395-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1395-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1395-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1395-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b1395-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1395-120">Request headers</span></span>
|<span data-ttu-id="b1395-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1395-121">Header</span></span>|<span data-ttu-id="b1395-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1395-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1395-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1395-123">Authorization</span></span>|<span data-ttu-id="b1395-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1395-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1395-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1395-125">Accept</span></span>|<span data-ttu-id="b1395-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1395-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1395-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1395-127">Request body</span></span>
<span data-ttu-id="b1395-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1395-128">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b1395-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b1395-129">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="b1395-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1395-130">Property</span></span>|<span data-ttu-id="b1395-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1395-131">Type</span></span>|<span data-ttu-id="b1395-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1395-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1395-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1395-133">roleScopeTagIds</span></span>|<span data-ttu-id="b1395-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b1395-134">String collection</span></span>|<span data-ttu-id="b1395-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b1395-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1395-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-137">id</span><span class="sxs-lookup"><span data-stu-id="b1395-137">id</span></span>|<span data-ttu-id="b1395-138">String</span><span class="sxs-lookup"><span data-stu-id="b1395-138">String</span></span>|<span data-ttu-id="b1395-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1395-139">Key of the entity.</span></span> <span data-ttu-id="b1395-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1395-141">createdDateTime</span></span>|<span data-ttu-id="b1395-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1395-142">DateTimeOffset</span></span>|<span data-ttu-id="b1395-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b1395-143">DateTime the object was created.</span></span> <span data-ttu-id="b1395-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-145">description</span><span class="sxs-lookup"><span data-stu-id="b1395-145">description</span></span>|<span data-ttu-id="b1395-146">String</span><span class="sxs-lookup"><span data-stu-id="b1395-146">String</span></span>|<span data-ttu-id="b1395-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1395-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1395-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1395-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b1395-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1395-150">DateTimeOffset</span></span>|<span data-ttu-id="b1395-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b1395-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b1395-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b1395-153">displayName</span></span>|<span data-ttu-id="b1395-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1395-154">String</span></span>|<span data-ttu-id="b1395-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1395-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1395-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-157">version</span><span class="sxs-lookup"><span data-stu-id="b1395-157">version</span></span>|<span data-ttu-id="b1395-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-158">Int32</span></span>|<span data-ttu-id="b1395-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1395-159">Version of the device configuration.</span></span> <span data-ttu-id="b1395-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b1395-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b1395-161">passwordRequired</span></span>|<span data-ttu-id="b1395-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-162">Boolean</span></span>|<span data-ttu-id="b1395-163">Exige uma senha para desbloquear o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1395-163">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b1395-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b1395-164">passwordMinimumLength</span></span>|<span data-ttu-id="b1395-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-165">Int32</span></span>|<span data-ttu-id="b1395-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b1395-166">Minimum password length.</span></span> <span data-ttu-id="b1395-167">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="b1395-167">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b1395-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b1395-168">passwordRequiredType</span></span>|[<span data-ttu-id="b1395-169">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b1395-169">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="b1395-170">Tipo de caracteres em senha.</span><span class="sxs-lookup"><span data-stu-id="b1395-170">Type of characters in password.</span></span> <span data-ttu-id="b1395-171">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="b1395-171">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b1395-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b1395-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b1395-173">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-173">Int32</span></span>|<span data-ttu-id="b1395-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="b1395-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b1395-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b1395-175">passwordExpirationDays</span></span>|<span data-ttu-id="b1395-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-176">Int32</span></span>|<span data-ttu-id="b1395-177">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="b1395-177">Number of days before the password expires.</span></span> <span data-ttu-id="b1395-178">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="b1395-178">Valid values 1 to 365</span></span>|
|<span data-ttu-id="b1395-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b1395-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b1395-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-180">Int32</span></span>|<span data-ttu-id="b1395-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="b1395-181">Number of previous passwords to block.</span></span> <span data-ttu-id="b1395-182">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="b1395-182">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b1395-183">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b1395-183">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b1395-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b1395-184">Int32</span></span>|<span data-ttu-id="b1395-185">Número de falhas de entrada permitidas antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b1395-185">Number of sign-in failures allowed before factory reset.</span></span> <span data-ttu-id="b1395-186">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="b1395-186">Valid values 1 to 16</span></span>|
|<span data-ttu-id="b1395-187">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b1395-187">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b1395-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-188">Boolean</span></span>|<span data-ttu-id="b1395-189">Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="b1395-189">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b1395-190">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b1395-190">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b1395-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-191">Boolean</span></span>|<span data-ttu-id="b1395-192">Desabilite a depuração USB em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="b1395-192">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b1395-193">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b1395-193">securityRequireVerifyApps</span></span>|<span data-ttu-id="b1395-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-194">Boolean</span></span>|<span data-ttu-id="b1395-195">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="b1395-195">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b1395-196">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b1395-196">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b1395-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-197">Boolean</span></span>|<span data-ttu-id="b1395-198">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="b1395-198">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b1395-199">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1395-199">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1395-200">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1395-200">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1395-201">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="b1395-201">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1395-202">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b1395-202">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1395-203">advancedThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b1395-203">advancedThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b1395-204">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b1395-204">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="b1395-205">MDATP requer nível mínimo de risco de proteção contra ameaças móveis para relatar não conformidade.</span><span class="sxs-lookup"><span data-stu-id="b1395-205">MDATP Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b1395-206">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="b1395-206">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b1395-207">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b1395-207">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b1395-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-208">Boolean</span></span>|<span data-ttu-id="b1395-209">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="b1395-209">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b1395-210">securityBlockDeviceAdministratorManagedDevices</span><span class="sxs-lookup"><span data-stu-id="b1395-210">securityBlockDeviceAdministratorManagedDevices</span></span>|<span data-ttu-id="b1395-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-211">Boolean</span></span>|<span data-ttu-id="b1395-212">Bloquear dispositivos gerenciados pelo administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b1395-212">Block device administrator managed devices.</span></span>|
|<span data-ttu-id="b1395-213">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b1395-213">osMinimumVersion</span></span>|<span data-ttu-id="b1395-214">String</span><span class="sxs-lookup"><span data-stu-id="b1395-214">String</span></span>|<span data-ttu-id="b1395-215">Versão mínima do Android.</span><span class="sxs-lookup"><span data-stu-id="b1395-215">Minimum Android version.</span></span>|
|<span data-ttu-id="b1395-216">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b1395-216">osMaximumVersion</span></span>|<span data-ttu-id="b1395-217">String</span><span class="sxs-lookup"><span data-stu-id="b1395-217">String</span></span>|<span data-ttu-id="b1395-218">Versão máxima do Android.</span><span class="sxs-lookup"><span data-stu-id="b1395-218">Maximum Android version.</span></span>|
|<span data-ttu-id="b1395-219">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b1395-219">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b1395-220">String</span><span class="sxs-lookup"><span data-stu-id="b1395-220">String</span></span>|<span data-ttu-id="b1395-221">Nível mínimo de patch de segurança Android.</span><span class="sxs-lookup"><span data-stu-id="b1395-221">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b1395-222">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b1395-222">storageRequireEncryption</span></span>|<span data-ttu-id="b1395-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-223">Boolean</span></span>|<span data-ttu-id="b1395-224">Exige criptografia em dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="b1395-224">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b1395-225">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b1395-225">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b1395-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-226">Boolean</span></span>|<span data-ttu-id="b1395-227">Exige que o dispositivo passe na verificação de integridade básica SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b1395-227">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b1395-228">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b1395-228">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b1395-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-229">Boolean</span></span>|<span data-ttu-id="b1395-230">Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.</span><span class="sxs-lookup"><span data-stu-id="b1395-230">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b1395-231">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b1395-231">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b1395-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-232">Boolean</span></span>|<span data-ttu-id="b1395-233">Exige que os Google Play Services sejam instalados e habilitados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1395-233">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b1395-234">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b1395-234">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b1395-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-235">Boolean</span></span>|<span data-ttu-id="b1395-236">Exige que o dispositivo tenha provedores de segurança atualizados.</span><span class="sxs-lookup"><span data-stu-id="b1395-236">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b1395-237">O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.</span><span class="sxs-lookup"><span data-stu-id="b1395-237">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b1395-238">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b1395-238">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b1395-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1395-239">Boolean</span></span>|<span data-ttu-id="b1395-240">Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="b1395-240">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|
|<span data-ttu-id="b1395-241">conditionStatementId</span><span class="sxs-lookup"><span data-stu-id="b1395-241">conditionStatementId</span></span>|<span data-ttu-id="b1395-242">String</span><span class="sxs-lookup"><span data-stu-id="b1395-242">String</span></span>|<span data-ttu-id="b1395-243">ID da instrução de condição.</span><span class="sxs-lookup"><span data-stu-id="b1395-243">Condition statement id.</span></span>|
|<span data-ttu-id="b1395-244">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="b1395-244">restrictedApps</span></span>|<span data-ttu-id="b1395-245">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b1395-245">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b1395-246">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="b1395-246">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="b1395-247">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="b1395-247">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b1395-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1395-248">Response</span></span>
<span data-ttu-id="b1395-249">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1395-249">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune-deviceconfig-androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1395-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1395-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1395-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1395-251">Request</span></span>
<span data-ttu-id="b1395-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1395-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1710

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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
  "securityBlockDeviceAdministratorManagedDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b1395-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1395-253">Response</span></span>
<span data-ttu-id="b1395-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1395-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1882

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
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
  "securityBlockDeviceAdministratorManagedDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true,
  "conditionStatementId": "Condition Statement Id value",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```



