---
title: Criar iosCompliancePolicy
description: Cria um novo objeto iosCompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 79d99fb2c0cabb3ca2399eaf6d74d8cad1de49e8
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895312"
---
# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="f334b-103">Criar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f334b-103">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="f334b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f334b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f334b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f334b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f334b-106">Cria um novo objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f334b-106">Create a new [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f334b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f334b-107">Prerequisites</span></span>
<span data-ttu-id="f334b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f334b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f334b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f334b-110">Permission type</span></span>|<span data-ttu-id="f334b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f334b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f334b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f334b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f334b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f334b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f334b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f334b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f334b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f334b-115">Not supported.</span></span>|
|<span data-ttu-id="f334b-116">Application</span><span class="sxs-lookup"><span data-stu-id="f334b-116">Application</span></span>|<span data-ttu-id="f334b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f334b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f334b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f334b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="f334b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f334b-119">Request headers</span></span>
|<span data-ttu-id="f334b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f334b-120">Header</span></span>|<span data-ttu-id="f334b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f334b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f334b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f334b-122">Authorization</span></span>|<span data-ttu-id="f334b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f334b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f334b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f334b-124">Accept</span></span>|<span data-ttu-id="f334b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f334b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f334b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f334b-126">Request body</span></span>
<span data-ttu-id="f334b-127">No corpo da solicitação, forneça uma representação JSON do objeto iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f334b-127">In the request body, supply a JSON representation for the iosCompliancePolicy object.</span></span>

<span data-ttu-id="f334b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosCompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="f334b-128">The following table shows the properties that are required when you create the iosCompliancePolicy.</span></span>

|<span data-ttu-id="f334b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f334b-129">Property</span></span>|<span data-ttu-id="f334b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f334b-130">Type</span></span>|<span data-ttu-id="f334b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f334b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f334b-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f334b-132">roleScopeTagIds</span></span>|<span data-ttu-id="f334b-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f334b-133">String collection</span></span>|<span data-ttu-id="f334b-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f334b-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f334b-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f334b-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f334b-136">descrição</span><span class="sxs-lookup"><span data-stu-id="f334b-136">description</span></span>|<span data-ttu-id="f334b-137">String</span><span class="sxs-lookup"><span data-stu-id="f334b-137">String</span></span>|<span data-ttu-id="f334b-138">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f334b-138">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f334b-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f334b-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f334b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="f334b-140">displayName</span></span>|<span data-ttu-id="f334b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f334b-141">String</span></span>|<span data-ttu-id="f334b-142">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f334b-142">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f334b-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f334b-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f334b-144">version</span><span class="sxs-lookup"><span data-stu-id="f334b-144">version</span></span>|<span data-ttu-id="f334b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-145">Int32</span></span>|<span data-ttu-id="f334b-146">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f334b-146">Version of the device configuration.</span></span> <span data-ttu-id="f334b-147">Herdado de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f334b-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f334b-148">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f334b-148">passcodeBlockSimple</span></span>|<span data-ttu-id="f334b-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="f334b-149">Boolean</span></span>|<span data-ttu-id="f334b-150">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f334b-150">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f334b-151">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f334b-151">passcodeExpirationDays</span></span>|<span data-ttu-id="f334b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-152">Int32</span></span>|<span data-ttu-id="f334b-153">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="f334b-153">Number of days before the passcode expires.</span></span> <span data-ttu-id="f334b-154">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="f334b-154">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f334b-155">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f334b-155">passcodeMinimumLength</span></span>|<span data-ttu-id="f334b-156">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-156">Int32</span></span>|<span data-ttu-id="f334b-157">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="f334b-157">Minimum length of passcode.</span></span> <span data-ttu-id="f334b-158">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="f334b-158">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f334b-159">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f334b-159">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f334b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-160">Int32</span></span>|<span data-ttu-id="f334b-161">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="f334b-161">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f334b-162">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f334b-162">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f334b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-163">Int32</span></span>|<span data-ttu-id="f334b-164">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f334b-164">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f334b-165">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f334b-165">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f334b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-166">Int32</span></span>|<span data-ttu-id="f334b-167">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f334b-167">Number of previous passcodes to block.</span></span> <span data-ttu-id="f334b-168">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="f334b-168">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f334b-169">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f334b-169">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f334b-170">Int32</span><span class="sxs-lookup"><span data-stu-id="f334b-170">Int32</span></span>|<span data-ttu-id="f334b-171">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="f334b-171">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f334b-172">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f334b-172">passcodeRequiredType</span></span>|[<span data-ttu-id="f334b-173">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f334b-173">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f334b-174">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f334b-174">The required passcode type.</span></span> <span data-ttu-id="f334b-175">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f334b-175">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f334b-176">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f334b-176">passcodeRequired</span></span>|<span data-ttu-id="f334b-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="f334b-177">Boolean</span></span>|<span data-ttu-id="f334b-178">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="f334b-178">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f334b-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f334b-179">osMinimumVersion</span></span>|<span data-ttu-id="f334b-180">String</span><span class="sxs-lookup"><span data-stu-id="f334b-180">String</span></span>|<span data-ttu-id="f334b-181">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="f334b-181">Minimum IOS version.</span></span>|
|<span data-ttu-id="f334b-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f334b-182">osMaximumVersion</span></span>|<span data-ttu-id="f334b-183">String</span><span class="sxs-lookup"><span data-stu-id="f334b-183">String</span></span>|<span data-ttu-id="f334b-184">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="f334b-184">Maximum IOS version.</span></span>|
|<span data-ttu-id="f334b-185">osMinimumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="f334b-185">osMinimumBuildVersion</span></span>|<span data-ttu-id="f334b-186">String</span><span class="sxs-lookup"><span data-stu-id="f334b-186">String</span></span>|<span data-ttu-id="f334b-187">Versão mínima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="f334b-187">Minimum IOS build version.</span></span>|
|<span data-ttu-id="f334b-188">osMaximumBuildVersion</span><span class="sxs-lookup"><span data-stu-id="f334b-188">osMaximumBuildVersion</span></span>|<span data-ttu-id="f334b-189">String</span><span class="sxs-lookup"><span data-stu-id="f334b-189">String</span></span>|<span data-ttu-id="f334b-190">Versão máxima do IOS Build.</span><span class="sxs-lookup"><span data-stu-id="f334b-190">Maximum IOS build version.</span></span>|
|<span data-ttu-id="f334b-191">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="f334b-191">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="f334b-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="f334b-192">Boolean</span></span>|<span data-ttu-id="f334b-193">Os dispositivos não devem ser violados ou com modificações root.</span><span class="sxs-lookup"><span data-stu-id="f334b-193">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="f334b-194">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f334b-194">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="f334b-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="f334b-195">Boolean</span></span>|<span data-ttu-id="f334b-196">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="f334b-196">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="f334b-197">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="f334b-197">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="f334b-198">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="f334b-198">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="f334b-199">Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="f334b-199">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="f334b-200">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="f334b-200">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="f334b-201">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="f334b-201">managedEmailProfileRequired</span></span>|<span data-ttu-id="f334b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="f334b-202">Boolean</span></span>|<span data-ttu-id="f334b-203">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="f334b-203">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="f334b-204">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="f334b-204">restrictedApps</span></span>|<span data-ttu-id="f334b-205">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f334b-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f334b-206">Exigir que o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="f334b-206">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="f334b-207">Essa coleção pode conter um máximo de 100 elementos.</span><span class="sxs-lookup"><span data-stu-id="f334b-207">This collection can contain a maximum of 100 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f334b-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="f334b-208">Response</span></span>
<span data-ttu-id="f334b-209">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f334b-209">If successful, this method returns a `201 Created` response code and a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f334b-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f334b-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="f334b-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f334b-211">Request</span></span>
<span data-ttu-id="f334b-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f334b-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f334b-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="f334b-213">Response</span></span>
<span data-ttu-id="f334b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f334b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






