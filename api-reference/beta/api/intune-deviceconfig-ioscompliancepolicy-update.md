---
title: Atualizar iosCompliancePolicy
description: Atualiza as propriedades de um objeto iosCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0010b938c6aab1e7271d32cd82d889f93d2e3223
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082704"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="e6548-103">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e6548-103">Update iosCompliancePolicy</span></span>

<span data-ttu-id="e6548-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6548-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6548-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6548-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6548-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6548-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6548-107">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6548-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6548-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6548-108">Prerequisites</span></span>
<span data-ttu-id="e6548-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6548-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6548-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6548-111">Permission type</span></span>|<span data-ttu-id="e6548-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6548-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6548-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6548-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6548-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6548-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6548-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6548-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6548-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6548-116">Not supported.</span></span>|
|<span data-ttu-id="e6548-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6548-117">Application</span></span>|<span data-ttu-id="e6548-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6548-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6548-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6548-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e6548-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6548-120">Request headers</span></span>
|<span data-ttu-id="e6548-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6548-121">Header</span></span>|<span data-ttu-id="e6548-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6548-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6548-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6548-123">Authorization</span></span>|<span data-ttu-id="e6548-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6548-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6548-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6548-125">Accept</span></span>|<span data-ttu-id="e6548-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6548-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6548-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6548-127">Request body</span></span>
<span data-ttu-id="e6548-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6548-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="e6548-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e6548-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="e6548-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6548-130">Property</span></span>|<span data-ttu-id="e6548-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6548-131">Type</span></span>|<span data-ttu-id="e6548-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6548-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6548-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6548-133">roleScopeTagIds</span></span>|<span data-ttu-id="e6548-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e6548-134">String collection</span></span>|<span data-ttu-id="e6548-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e6548-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6548-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-137">id</span><span class="sxs-lookup"><span data-stu-id="e6548-137">id</span></span>|<span data-ttu-id="e6548-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6548-138">String</span></span>|<span data-ttu-id="e6548-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6548-139">Key of the entity.</span></span> <span data-ttu-id="e6548-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6548-141">createdDateTime</span></span>|<span data-ttu-id="e6548-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6548-142">DateTimeOffset</span></span>|<span data-ttu-id="e6548-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e6548-143">DateTime the object was created.</span></span> <span data-ttu-id="e6548-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-145">description</span><span class="sxs-lookup"><span data-stu-id="e6548-145">description</span></span>|<span data-ttu-id="e6548-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6548-146">String</span></span>|<span data-ttu-id="e6548-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6548-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6548-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6548-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e6548-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6548-150">DateTimeOffset</span></span>|<span data-ttu-id="e6548-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e6548-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e6548-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e6548-153">displayName</span></span>|<span data-ttu-id="e6548-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6548-154">String</span></span>|<span data-ttu-id="e6548-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6548-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6548-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-157">version</span><span class="sxs-lookup"><span data-stu-id="e6548-157">version</span></span>|<span data-ttu-id="e6548-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-158">Int32</span></span>|<span data-ttu-id="e6548-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6548-159">Version of the device configuration.</span></span> <span data-ttu-id="e6548-160">Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e6548-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e6548-161">passcodeBlockSimple</span></span>|<span data-ttu-id="e6548-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6548-162">Boolean</span></span>|<span data-ttu-id="e6548-163">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e6548-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="e6548-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e6548-164">passcodeExpirationDays</span></span>|<span data-ttu-id="e6548-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-165">Int32</span></span>|<span data-ttu-id="e6548-166">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="e6548-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="e6548-167">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="e6548-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="e6548-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e6548-168">passcodeMinimumLength</span></span>|<span data-ttu-id="e6548-169">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-169">Int32</span></span>|<span data-ttu-id="e6548-170">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="e6548-170">Minimum length of passcode.</span></span> <span data-ttu-id="e6548-171">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="e6548-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="e6548-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e6548-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e6548-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-173">Int32</span></span>|<span data-ttu-id="e6548-174">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="e6548-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="e6548-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e6548-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e6548-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-176">Int32</span></span>|<span data-ttu-id="e6548-177">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e6548-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e6548-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="e6548-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="e6548-179">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-179">Int32</span></span>|<span data-ttu-id="e6548-180">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e6548-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="e6548-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="e6548-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="e6548-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e6548-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="e6548-183">Int32</span><span class="sxs-lookup"><span data-stu-id="e6548-183">Int32</span></span>|<span data-ttu-id="e6548-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="e6548-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e6548-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="e6548-185">passcodeRequiredType</span></span>|[<span data-ttu-id="e6548-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e6548-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e6548-187">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e6548-187">The required passcode type.</span></span> <span data-ttu-id="e6548-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e6548-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e6548-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="e6548-189">passcodeRequired</span></span>|<span data-ttu-id="e6548-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6548-190">Boolean</span></span>|<span data-ttu-id="e6548-191">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="e6548-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="e6548-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e6548-192">osMinimumVersion</span></span>|<span data-ttu-id="e6548-193">String</span><span class="sxs-lookup"><span data-stu-id="e6548-193">String</span></span>|<span data-ttu-id="e6548-194">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="e6548-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="e6548-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e6548-195">osMaximumVersion</span></span>|<span data-ttu-id="e6548-196">String</span><span class="sxs-lookup"><span data-stu-id="e6548-196">String</span></span>|<span data-ttu-id="e6548-197">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="e6548-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="e6548-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e6548-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="e6548-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6548-199">String</span></span>|<span data-ttu-id="e6548-200">Versão mínima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="e6548-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="e6548-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="e6548-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="e6548-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6548-202">String</span></span>|<span data-ttu-id="e6548-203">Versão máxima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="e6548-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="e6548-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="e6548-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="e6548-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6548-205">Boolean</span></span>|<span data-ttu-id="e6548-206">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="e6548-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="e6548-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="e6548-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="e6548-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6548-208">Boolean</span></span>|<span data-ttu-id="e6548-209">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="e6548-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="e6548-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="e6548-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="e6548-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="e6548-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="e6548-212">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="e6548-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="e6548-213">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="e6548-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="e6548-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="e6548-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="e6548-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6548-215">Boolean</span></span>|<span data-ttu-id="e6548-216">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="e6548-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="e6548-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e6548-217">restrictedApps</span></span>|<span data-ttu-id="e6548-218">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="e6548-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e6548-219">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="e6548-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="e6548-220">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="e6548-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e6548-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6548-221">Response</span></span>
<span data-ttu-id="e6548-222">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6548-222">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6548-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6548-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6548-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6548-224">Request</span></span>
<span data-ttu-id="e6548-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6548-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
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

### <a name="response"></a><span data-ttu-id="e6548-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6548-226">Response</span></span>
<span data-ttu-id="e6548-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6548-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
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






