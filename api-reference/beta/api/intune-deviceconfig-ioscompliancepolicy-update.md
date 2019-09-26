---
title: Atualizar iosCompliancePolicy
description: Atualiza as propriedades de um objeto iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 92610be52eed55725eb525f82121ebe715c62c11
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167995"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="6442e-103">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6442e-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="6442e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6442e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6442e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6442e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6442e-106">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6442e-106">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6442e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6442e-107">Prerequisites</span></span>
<span data-ttu-id="6442e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6442e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6442e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6442e-110">Permission type</span></span>|<span data-ttu-id="6442e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6442e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6442e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6442e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6442e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6442e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6442e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6442e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6442e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6442e-115">Not supported.</span></span>|
|<span data-ttu-id="6442e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6442e-116">Application</span></span>|<span data-ttu-id="6442e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6442e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6442e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6442e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6442e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6442e-119">Request headers</span></span>
|<span data-ttu-id="6442e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6442e-120">Header</span></span>|<span data-ttu-id="6442e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6442e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6442e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6442e-122">Authorization</span></span>|<span data-ttu-id="6442e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6442e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6442e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6442e-124">Accept</span></span>|<span data-ttu-id="6442e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6442e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6442e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6442e-126">Request body</span></span>
<span data-ttu-id="6442e-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6442e-127">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6442e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6442e-128">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="6442e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6442e-129">Property</span></span>|<span data-ttu-id="6442e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6442e-130">Type</span></span>|<span data-ttu-id="6442e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6442e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6442e-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6442e-132">roleScopeTagIds</span></span>|<span data-ttu-id="6442e-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6442e-133">String collection</span></span>|<span data-ttu-id="6442e-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6442e-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6442e-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-136">id</span><span class="sxs-lookup"><span data-stu-id="6442e-136">id</span></span>|<span data-ttu-id="6442e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6442e-137">String</span></span>|<span data-ttu-id="6442e-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6442e-138">Key of the entity.</span></span> <span data-ttu-id="6442e-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6442e-140">createdDateTime</span></span>|<span data-ttu-id="6442e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6442e-141">DateTimeOffset</span></span>|<span data-ttu-id="6442e-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6442e-142">DateTime the object was created.</span></span> <span data-ttu-id="6442e-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-144">descrição</span><span class="sxs-lookup"><span data-stu-id="6442e-144">description</span></span>|<span data-ttu-id="6442e-145">String</span><span class="sxs-lookup"><span data-stu-id="6442e-145">String</span></span>|<span data-ttu-id="6442e-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6442e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6442e-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6442e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6442e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6442e-149">DateTimeOffset</span></span>|<span data-ttu-id="6442e-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6442e-150">DateTime the object was last modified.</span></span> <span data-ttu-id="6442e-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="6442e-152">displayName</span></span>|<span data-ttu-id="6442e-153">String</span><span class="sxs-lookup"><span data-stu-id="6442e-153">String</span></span>|<span data-ttu-id="6442e-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6442e-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6442e-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-156">version</span><span class="sxs-lookup"><span data-stu-id="6442e-156">version</span></span>|<span data-ttu-id="6442e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-157">Int32</span></span>|<span data-ttu-id="6442e-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6442e-158">Version of the device configuration.</span></span> <span data-ttu-id="6442e-159">Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6442e-160">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6442e-160">passcodeBlockSimple</span></span>|<span data-ttu-id="6442e-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="6442e-161">Boolean</span></span>|<span data-ttu-id="6442e-162">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6442e-162">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6442e-163">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6442e-163">passcodeExpirationDays</span></span>|<span data-ttu-id="6442e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-164">Int32</span></span>|<span data-ttu-id="6442e-165">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6442e-165">Number of days before the passcode expires.</span></span> <span data-ttu-id="6442e-166">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="6442e-166">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6442e-167">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6442e-167">passcodeMinimumLength</span></span>|<span data-ttu-id="6442e-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-168">Int32</span></span>|<span data-ttu-id="6442e-169">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="6442e-169">Minimum length of passcode.</span></span> <span data-ttu-id="6442e-170">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="6442e-170">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6442e-171">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6442e-171">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6442e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-172">Int32</span></span>|<span data-ttu-id="6442e-173">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="6442e-173">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6442e-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6442e-174">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6442e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-175">Int32</span></span>|<span data-ttu-id="6442e-176">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6442e-176">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6442e-177">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6442e-177">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6442e-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-178">Int32</span></span>|<span data-ttu-id="6442e-179">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="6442e-179">Number of previous passcodes to block.</span></span> <span data-ttu-id="6442e-180">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="6442e-180">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6442e-181">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6442e-181">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6442e-182">Int32</span><span class="sxs-lookup"><span data-stu-id="6442e-182">Int32</span></span>|<span data-ttu-id="6442e-183">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="6442e-183">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6442e-184">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6442e-184">passcodeRequiredType</span></span>|[<span data-ttu-id="6442e-185">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6442e-185">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6442e-186">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="6442e-186">The required passcode type.</span></span> <span data-ttu-id="6442e-187">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6442e-187">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6442e-188">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6442e-188">passcodeRequired</span></span>|<span data-ttu-id="6442e-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="6442e-189">Boolean</span></span>|<span data-ttu-id="6442e-190">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="6442e-190">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6442e-191">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6442e-191">osMinimumVersion</span></span>|<span data-ttu-id="6442e-192">String</span><span class="sxs-lookup"><span data-stu-id="6442e-192">String</span></span>|<span data-ttu-id="6442e-193">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="6442e-193">Minimum IOS version.</span></span>|
|<span data-ttu-id="6442e-194">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6442e-194">osMaximumVersion</span></span>|<span data-ttu-id="6442e-195">String</span><span class="sxs-lookup"><span data-stu-id="6442e-195">String</span></span>|<span data-ttu-id="6442e-196">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="6442e-196">Maximum IOS version.</span></span>|
|<span data-ttu-id="6442e-197">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6442e-197">osMinimumBuildVersion</span></span>|<span data-ttu-id="6442e-198">String</span><span class="sxs-lookup"><span data-stu-id="6442e-198">String</span></span>|<span data-ttu-id="6442e-199">Versão mínima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="6442e-199">Minimum IOS build version.</span></span>|
|<span data-ttu-id="6442e-200">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="6442e-200">osMaximumBuildVersion</span></span>|<span data-ttu-id="6442e-201">String</span><span class="sxs-lookup"><span data-stu-id="6442e-201">String</span></span>|<span data-ttu-id="6442e-202">Versão máxima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="6442e-202">Maximum IOS build version.</span></span>|
|<span data-ttu-id="6442e-203">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="6442e-203">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="6442e-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="6442e-204">Boolean</span></span>|<span data-ttu-id="6442e-205">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="6442e-205">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="6442e-206">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6442e-206">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6442e-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="6442e-207">Boolean</span></span>|<span data-ttu-id="6442e-208">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="6442e-208">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6442e-209">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6442e-209">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="6442e-210">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="6442e-210">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="6442e-211">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6442e-211">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6442e-212">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="6442e-212">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6442e-213">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="6442e-213">managedEmailProfileRequired</span></span>|<span data-ttu-id="6442e-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="6442e-214">Boolean</span></span>|<span data-ttu-id="6442e-215">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="6442e-215">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="6442e-216">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6442e-216">restrictedApps</span></span>|<span data-ttu-id="6442e-217">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6442e-217">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6442e-218">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="6442e-218">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="6442e-219">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="6442e-219">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6442e-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="6442e-220">Response</span></span>
<span data-ttu-id="6442e-221">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6442e-221">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6442e-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6442e-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6442e-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6442e-223">Request</span></span>
<span data-ttu-id="6442e-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6442e-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6442e-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="6442e-225">Response</span></span>
<span data-ttu-id="6442e-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6442e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




