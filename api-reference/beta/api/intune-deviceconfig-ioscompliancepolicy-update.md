---
title: Atualizar iosCompliancePolicy
description: Atualiza as propriedades de um objeto iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b778259b944a81b6648d9ef167a0f9d1f70f5e6e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467530"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="6c1a2-103">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6c1a2-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="6c1a2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c1a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c1a2-106">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c1a2-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c1a2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c1a2-107">Prerequisites</span></span>
<span data-ttu-id="6c1a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c1a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c1a2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c1a2-110">Permission type</span></span>|<span data-ttu-id="6c1a2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c1a2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c1a2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c1a2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c1a2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c1a2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-115">Not supported.</span></span>|
|<span data-ttu-id="6c1a2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c1a2-116">Application</span></span>|<span data-ttu-id="6c1a2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c1a2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c1a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6c1a2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c1a2-119">Request headers</span></span>
|<span data-ttu-id="6c1a2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c1a2-120">Header</span></span>|<span data-ttu-id="6c1a2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c1a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c1a2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c1a2-122">Authorization</span></span>|<span data-ttu-id="6c1a2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c1a2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c1a2-124">Accept</span></span>|<span data-ttu-id="6c1a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c1a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c1a2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c1a2-126">Request body</span></span>
<span data-ttu-id="6c1a2-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c1a2-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6c1a2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c1a2-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="6c1a2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c1a2-129">Property</span></span>|<span data-ttu-id="6c1a2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c1a2-130">Type</span></span>|<span data-ttu-id="6c1a2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c1a2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c1a2-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c1a2-132">roleScopeTagIds</span></span>|<span data-ttu-id="6c1a2-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c1a2-133">String collection</span></span>|<span data-ttu-id="6c1a2-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c1a2-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-136">id</span><span class="sxs-lookup"><span data-stu-id="6c1a2-136">id</span></span>|<span data-ttu-id="6c1a2-137">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-137">String</span></span>|<span data-ttu-id="6c1a2-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-138">Key of the entity.</span></span> <span data-ttu-id="6c1a2-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c1a2-140">createdDateTime</span></span>|<span data-ttu-id="6c1a2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c1a2-141">DateTimeOffset</span></span>|<span data-ttu-id="6c1a2-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-142">DateTime the object was created.</span></span> <span data-ttu-id="6c1a2-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-144">description</span><span class="sxs-lookup"><span data-stu-id="6c1a2-144">description</span></span>|<span data-ttu-id="6c1a2-145">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-145">String</span></span>|<span data-ttu-id="6c1a2-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c1a2-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c1a2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6c1a2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c1a2-149">DateTimeOffset</span></span>|<span data-ttu-id="6c1a2-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6c1a2-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6c1a2-152">displayName</span></span>|<span data-ttu-id="6c1a2-153">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-153">String</span></span>|<span data-ttu-id="6c1a2-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c1a2-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-156">version</span><span class="sxs-lookup"><span data-stu-id="6c1a2-156">version</span></span>|<span data-ttu-id="6c1a2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-157">Int32</span></span>|<span data-ttu-id="6c1a2-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-158">Version of the device configuration.</span></span> <span data-ttu-id="6c1a2-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6c1a2-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6c1a2-160">passcodeBlockSimple</span></span>|<span data-ttu-id="6c1a2-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c1a2-161">Boolean</span></span>|<span data-ttu-id="6c1a2-162">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6c1a2-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6c1a2-163">passcodeExpirationDays</span></span>|<span data-ttu-id="6c1a2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-164">Int32</span></span>|<span data-ttu-id="6c1a2-165">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="6c1a2-166">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="6c1a2-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6c1a2-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6c1a2-167">passcodeMinimumLength</span></span>|<span data-ttu-id="6c1a2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-168">Int32</span></span>|<span data-ttu-id="6c1a2-169">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-169">Minimum length of passcode.</span></span> <span data-ttu-id="6c1a2-170">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="6c1a2-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6c1a2-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6c1a2-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6c1a2-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-172">Int32</span></span>|<span data-ttu-id="6c1a2-173">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6c1a2-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6c1a2-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6c1a2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-175">Int32</span></span>|<span data-ttu-id="6c1a2-176">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6c1a2-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6c1a2-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6c1a2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-178">Int32</span></span>|<span data-ttu-id="6c1a2-179">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="6c1a2-180">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="6c1a2-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6c1a2-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6c1a2-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6c1a2-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6c1a2-182">Int32</span></span>|<span data-ttu-id="6c1a2-183">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6c1a2-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6c1a2-184">passcodeRequiredType</span></span>|[<span data-ttu-id="6c1a2-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6c1a2-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6c1a2-186">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-186">The required passcode type.</span></span> <span data-ttu-id="6c1a2-187">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6c1a2-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6c1a2-188">passcodeRequired</span></span>|<span data-ttu-id="6c1a2-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c1a2-189">Boolean</span></span>|<span data-ttu-id="6c1a2-190">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6c1a2-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6c1a2-191">osMinimumVersion</span></span>|<span data-ttu-id="6c1a2-192">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-192">String</span></span>|<span data-ttu-id="6c1a2-193">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="6c1a2-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6c1a2-194">osMaximumVersion</span></span>|<span data-ttu-id="6c1a2-195">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-195">String</span></span>|<span data-ttu-id="6c1a2-196">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="6c1a2-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6c1a2-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="6c1a2-198">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-198">String</span></span>|<span data-ttu-id="6c1a2-199">Versão mínima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="6c1a2-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6c1a2-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="6c1a2-201">String</span><span class="sxs-lookup"><span data-stu-id="6c1a2-201">String</span></span>|<span data-ttu-id="6c1a2-202">Versão máxima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="6c1a2-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6c1a2-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6c1a2-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c1a2-204">Boolean</span></span>|<span data-ttu-id="6c1a2-205">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6c1a2-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6c1a2-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6c1a2-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c1a2-207">Boolean</span></span>|<span data-ttu-id="6c1a2-208">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6c1a2-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6c1a2-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6c1a2-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6c1a2-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6c1a2-211">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6c1a2-212">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6c1a2-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="6c1a2-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="6c1a2-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c1a2-214">Boolean</span></span>|<span data-ttu-id="6c1a2-215">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="6c1a2-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6c1a2-216">restrictedApps</span></span>|<span data-ttu-id="6c1a2-217">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c1a2-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6c1a2-218">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="6c1a2-219">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6c1a2-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c1a2-220">Response</span></span>
<span data-ttu-id="6c1a2-221">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c1a2-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c1a2-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c1a2-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c1a2-223">Request</span></span>
<span data-ttu-id="6c1a2-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c1a2-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c1a2-225">Response</span></span>
<span data-ttu-id="6c1a2-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





