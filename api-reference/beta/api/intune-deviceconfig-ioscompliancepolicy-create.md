---
title: Criar iosCompliancePolicy
description: Cria um novo objeto iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ce2abd418d96598f617897c112c36ac70093d3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449051"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="c69b7-103">Criar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c69b7-103">Create iosCompliancePolicy</span></span>

<span data-ttu-id="c69b7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c69b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c69b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c69b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c69b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c69b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c69b7-107">Cria um novo objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="c69b7-107">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c69b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c69b7-108">Prerequisites</span></span>
<span data-ttu-id="c69b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c69b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c69b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c69b7-111">Permission type</span></span>|<span data-ttu-id="c69b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c69b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c69b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c69b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c69b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c69b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c69b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c69b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c69b7-116">Not supported.</span></span>|
|<span data-ttu-id="c69b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c69b7-117">Application</span></span>|<span data-ttu-id="c69b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c69b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c69b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="c69b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c69b7-120">Request headers</span></span>
|<span data-ttu-id="c69b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c69b7-121">Header</span></span>|<span data-ttu-id="c69b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c69b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c69b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c69b7-123">Authorization</span></span>|<span data-ttu-id="c69b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c69b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c69b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c69b7-125">Accept</span></span>|<span data-ttu-id="c69b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c69b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c69b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c69b7-127">Request body</span></span>
<span data-ttu-id="c69b7-128">No corpo da solicitação, forneça uma representação JSON do objeto iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c69b7-128">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="c69b7-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="c69b7-129">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="c69b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c69b7-130">Property</span></span>|<span data-ttu-id="c69b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c69b7-131">Type</span></span>|<span data-ttu-id="c69b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c69b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c69b7-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c69b7-133">roleScopeTagIds</span></span>|<span data-ttu-id="c69b7-134">String collection</span><span class="sxs-lookup"><span data-stu-id="c69b7-134">String collection</span></span>|<span data-ttu-id="c69b7-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c69b7-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c69b7-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-137">id</span><span class="sxs-lookup"><span data-stu-id="c69b7-137">id</span></span>|<span data-ttu-id="c69b7-138">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-138">String</span></span>|<span data-ttu-id="c69b7-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c69b7-139">Key of the entity.</span></span> <span data-ttu-id="c69b7-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c69b7-141">createdDateTime</span></span>|<span data-ttu-id="c69b7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c69b7-142">DateTimeOffset</span></span>|<span data-ttu-id="c69b7-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c69b7-143">DateTime the object was created.</span></span> <span data-ttu-id="c69b7-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-145">description</span><span class="sxs-lookup"><span data-stu-id="c69b7-145">description</span></span>|<span data-ttu-id="c69b7-146">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-146">String</span></span>|<span data-ttu-id="c69b7-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c69b7-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c69b7-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c69b7-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c69b7-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c69b7-150">DateTimeOffset</span></span>|<span data-ttu-id="c69b7-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c69b7-151">DateTime the object was last modified.</span></span> <span data-ttu-id="c69b7-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-153">displayName</span><span class="sxs-lookup"><span data-stu-id="c69b7-153">displayName</span></span>|<span data-ttu-id="c69b7-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c69b7-154">String</span></span>|<span data-ttu-id="c69b7-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c69b7-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c69b7-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-157">version</span><span class="sxs-lookup"><span data-stu-id="c69b7-157">version</span></span>|<span data-ttu-id="c69b7-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-158">Int32</span></span>|<span data-ttu-id="c69b7-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c69b7-159">Version of the device configuration.</span></span> <span data-ttu-id="c69b7-160">Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="c69b7-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c69b7-161">passcodeBlockSimple</span></span>|<span data-ttu-id="c69b7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c69b7-162">Boolean</span></span>|<span data-ttu-id="c69b7-163">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c69b7-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="c69b7-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c69b7-164">passcodeExpirationDays</span></span>|<span data-ttu-id="c69b7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-165">Int32</span></span>|<span data-ttu-id="c69b7-166">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="c69b7-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="c69b7-167">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="c69b7-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="c69b7-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c69b7-168">passcodeMinimumLength</span></span>|<span data-ttu-id="c69b7-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-169">Int32</span></span>|<span data-ttu-id="c69b7-170">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="c69b7-170">Minimum length of passcode.</span></span> <span data-ttu-id="c69b7-171">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="c69b7-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="c69b7-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c69b7-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c69b7-173">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-173">Int32</span></span>|<span data-ttu-id="c69b7-174">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="c69b7-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="c69b7-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c69b7-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c69b7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-176">Int32</span></span>|<span data-ttu-id="c69b7-177">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="c69b7-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c69b7-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="c69b7-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="c69b7-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-179">Int32</span></span>|<span data-ttu-id="c69b7-180">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="c69b7-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="c69b7-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="c69b7-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="c69b7-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c69b7-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="c69b7-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c69b7-183">Int32</span></span>|<span data-ttu-id="c69b7-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="c69b7-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c69b7-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="c69b7-185">passcodeRequiredType</span></span>|[<span data-ttu-id="c69b7-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c69b7-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c69b7-187">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="c69b7-187">The required passcode type.</span></span> <span data-ttu-id="c69b7-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c69b7-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c69b7-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="c69b7-189">passcodeRequired</span></span>|<span data-ttu-id="c69b7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c69b7-190">Boolean</span></span>|<span data-ttu-id="c69b7-191">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="c69b7-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="c69b7-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="c69b7-192">osMinimumVersion</span></span>|<span data-ttu-id="c69b7-193">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-193">String</span></span>|<span data-ttu-id="c69b7-194">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="c69b7-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="c69b7-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="c69b7-195">osMaximumVersion</span></span>|<span data-ttu-id="c69b7-196">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-196">String</span></span>|<span data-ttu-id="c69b7-197">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="c69b7-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="c69b7-198">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="c69b7-198">osMinimumBuildVersion</span></span>|<span data-ttu-id="c69b7-199">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-199">String</span></span>|<span data-ttu-id="c69b7-200">Versão mínima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="c69b7-200">Minimum IOS build version.</span></span>|
|<span data-ttu-id="c69b7-201">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="c69b7-201">osMaximumBuildVersion</span></span>|<span data-ttu-id="c69b7-202">String</span><span class="sxs-lookup"><span data-stu-id="c69b7-202">String</span></span>|<span data-ttu-id="c69b7-203">Versão máxima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="c69b7-203">Maximum IOS build version.</span></span>|
|<span data-ttu-id="c69b7-204">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="c69b7-204">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="c69b7-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c69b7-205">Boolean</span></span>|<span data-ttu-id="c69b7-206">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="c69b7-206">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="c69b7-207">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="c69b7-207">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="c69b7-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c69b7-208">Boolean</span></span>|<span data-ttu-id="c69b7-209">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="c69b7-209">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="c69b7-210">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c69b7-210">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="c69b7-211">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="c69b7-211">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="c69b7-212">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="c69b7-212">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="c69b7-213">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="c69b7-213">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="c69b7-214">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="c69b7-214">managedEmailProfileRequired</span></span>|<span data-ttu-id="c69b7-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="c69b7-215">Boolean</span></span>|<span data-ttu-id="c69b7-216">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="c69b7-216">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="c69b7-217">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c69b7-217">restrictedApps</span></span>|<span data-ttu-id="c69b7-218">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c69b7-218">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c69b7-219">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="c69b7-219">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="c69b7-220">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="c69b7-220">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c69b7-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69b7-221">Response</span></span>
<span data-ttu-id="c69b7-222">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c69b7-222">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c69b7-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c69b7-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="c69b7-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c69b7-224">Request</span></span>
<span data-ttu-id="c69b7-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c69b7-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="c69b7-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="c69b7-226">Response</span></span>
<span data-ttu-id="c69b7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c69b7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





