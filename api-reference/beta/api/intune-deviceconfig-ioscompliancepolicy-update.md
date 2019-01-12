---
title: Atualizar iosCompliancePolicy
description: Atualiza as propriedades de um objeto iosCompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a9ee2476d85ec1446fea4b45fac834eb62f82bc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967879"
---
# <a name="update-ioscompliancepolicy"></a><span data-ttu-id="138bd-103">Atualizar iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="138bd-103">Update iosCompliancePolicy</span></span>

> <span data-ttu-id="138bd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="138bd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="138bd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="138bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="138bd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="138bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="138bd-107">Atualiza as propriedades de um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="138bd-107">Update the properties of a [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="138bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="138bd-108">Prerequisites</span></span>
<span data-ttu-id="138bd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="138bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="138bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="138bd-111">Permission type</span></span>|<span data-ttu-id="138bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="138bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="138bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="138bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="138bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="138bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="138bd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="138bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="138bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="138bd-116">Not supported.</span></span>|
|<span data-ttu-id="138bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="138bd-117">Application</span></span>|<span data-ttu-id="138bd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="138bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="138bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="138bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="138bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="138bd-120">Request headers</span></span>
|<span data-ttu-id="138bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="138bd-121">Header</span></span>|<span data-ttu-id="138bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="138bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="138bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="138bd-123">Authorization</span></span>|<span data-ttu-id="138bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="138bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="138bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="138bd-125">Accept</span></span>|<span data-ttu-id="138bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="138bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="138bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="138bd-127">Request body</span></span>
<span data-ttu-id="138bd-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="138bd-128">In the request body, supply a JSON representation for the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object.</span></span>

<span data-ttu-id="138bd-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="138bd-129">The following table shows the properties that are required when you create the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).</span></span>

|<span data-ttu-id="138bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="138bd-130">Property</span></span>|<span data-ttu-id="138bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="138bd-131">Type</span></span>|<span data-ttu-id="138bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="138bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="138bd-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="138bd-133">roleScopeTagIds</span></span>|<span data-ttu-id="138bd-134">String collection</span><span class="sxs-lookup"><span data-stu-id="138bd-134">String collection</span></span>|<span data-ttu-id="138bd-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="138bd-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="138bd-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-137">id</span><span class="sxs-lookup"><span data-stu-id="138bd-137">id</span></span>|<span data-ttu-id="138bd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="138bd-138">String</span></span>|<span data-ttu-id="138bd-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="138bd-139">Key of the entity.</span></span> <span data-ttu-id="138bd-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="138bd-141">createdDateTime</span></span>|<span data-ttu-id="138bd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="138bd-142">DateTimeOffset</span></span>|<span data-ttu-id="138bd-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="138bd-143">DateTime the object was created.</span></span> <span data-ttu-id="138bd-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-145">description</span><span class="sxs-lookup"><span data-stu-id="138bd-145">description</span></span>|<span data-ttu-id="138bd-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="138bd-146">String</span></span>|<span data-ttu-id="138bd-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="138bd-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="138bd-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="138bd-149">lastModifiedDateTime</span></span>|<span data-ttu-id="138bd-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="138bd-150">DateTimeOffset</span></span>|<span data-ttu-id="138bd-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="138bd-151">DateTime the object was last modified.</span></span> <span data-ttu-id="138bd-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-153">displayName</span><span class="sxs-lookup"><span data-stu-id="138bd-153">displayName</span></span>|<span data-ttu-id="138bd-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="138bd-154">String</span></span>|<span data-ttu-id="138bd-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="138bd-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="138bd-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-157">version</span><span class="sxs-lookup"><span data-stu-id="138bd-157">version</span></span>|<span data-ttu-id="138bd-158">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-158">Int32</span></span>|<span data-ttu-id="138bd-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="138bd-159">Version of the device configuration.</span></span> <span data-ttu-id="138bd-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="138bd-161">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="138bd-161">passcodeBlockSimple</span></span>|<span data-ttu-id="138bd-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="138bd-162">Boolean</span></span>|<span data-ttu-id="138bd-163">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="138bd-163">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="138bd-164">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="138bd-164">passcodeExpirationDays</span></span>|<span data-ttu-id="138bd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-165">Int32</span></span>|<span data-ttu-id="138bd-166">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="138bd-166">Number of days before the passcode expires.</span></span> <span data-ttu-id="138bd-167">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="138bd-167">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="138bd-168">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="138bd-168">passcodeMinimumLength</span></span>|<span data-ttu-id="138bd-169">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-169">Int32</span></span>|<span data-ttu-id="138bd-170">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="138bd-170">Minimum length of passcode.</span></span> <span data-ttu-id="138bd-171">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="138bd-171">Valid values 4 to 14</span></span>|
|<span data-ttu-id="138bd-172">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="138bd-172">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="138bd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-173">Int32</span></span>|<span data-ttu-id="138bd-174">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="138bd-174">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="138bd-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="138bd-175">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="138bd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-176">Int32</span></span>|<span data-ttu-id="138bd-177">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="138bd-177">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="138bd-178">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="138bd-178">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="138bd-179">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-179">Int32</span></span>|<span data-ttu-id="138bd-180">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="138bd-180">Number of previous passcodes to block.</span></span> <span data-ttu-id="138bd-181">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="138bd-181">Valid values 1 to 24</span></span>|
|<span data-ttu-id="138bd-182">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="138bd-182">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="138bd-183">Int32</span><span class="sxs-lookup"><span data-stu-id="138bd-183">Int32</span></span>|<span data-ttu-id="138bd-184">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="138bd-184">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="138bd-185">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="138bd-185">passcodeRequiredType</span></span>|[<span data-ttu-id="138bd-186">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="138bd-186">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="138bd-187">O tipo de código de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="138bd-187">The required passcode type.</span></span> <span data-ttu-id="138bd-188">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="138bd-188">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="138bd-189">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="138bd-189">passcodeRequired</span></span>|<span data-ttu-id="138bd-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="138bd-190">Boolean</span></span>|<span data-ttu-id="138bd-191">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="138bd-191">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="138bd-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="138bd-192">osMinimumVersion</span></span>|<span data-ttu-id="138bd-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="138bd-193">String</span></span>|<span data-ttu-id="138bd-194">Versão mínima do IOS.</span><span class="sxs-lookup"><span data-stu-id="138bd-194">Minimum IOS version.</span></span>|
|<span data-ttu-id="138bd-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="138bd-195">osMaximumVersion</span></span>|<span data-ttu-id="138bd-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="138bd-196">String</span></span>|<span data-ttu-id="138bd-197">Versão máxima do iOS.</span><span class="sxs-lookup"><span data-stu-id="138bd-197">Maximum IOS version.</span></span>|
|<span data-ttu-id="138bd-198">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="138bd-198">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="138bd-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="138bd-199">Boolean</span></span>|<span data-ttu-id="138bd-200">Os dispositivos não podem ser desbloqueados ou modificados.</span><span class="sxs-lookup"><span data-stu-id="138bd-200">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="138bd-201">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="138bd-201">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="138bd-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="138bd-202">Boolean</span></span>|<span data-ttu-id="138bd-203">Exige que os dispositivos tenham habilitada a proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="138bd-203">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="138bd-204">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="138bd-204">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="138bd-205">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="138bd-205">deviceThreatProtectionLevel</span></span>](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|<span data-ttu-id="138bd-206">Exige o nível mínimo de risco de Proteção contra ameaças móveis para indicar falta de conformidade.</span><span class="sxs-lookup"><span data-stu-id="138bd-206">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="138bd-207">Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span><span class="sxs-lookup"><span data-stu-id="138bd-207">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="138bd-208">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="138bd-208">managedEmailProfileRequired</span></span>|<span data-ttu-id="138bd-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="138bd-209">Boolean</span></span>|<span data-ttu-id="138bd-210">Indica se um perfil de email gerenciado deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="138bd-210">Indicates whether or not to require a managed email profile.</span></span>|
|<span data-ttu-id="138bd-211">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="138bd-211">restrictedApps</span></span>|<span data-ttu-id="138bd-212">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="138bd-212">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="138bd-213">Exigir o dispositivo não tenha os aplicativos especificados instalados.</span><span class="sxs-lookup"><span data-stu-id="138bd-213">Require the device to not have the specified apps installed.</span></span> <span data-ttu-id="138bd-214">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="138bd-214">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="138bd-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="138bd-215">Response</span></span>
<span data-ttu-id="138bd-216">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="138bd-216">If successful, this method returns a `200 OK` response code and an updated [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="138bd-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="138bd-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="138bd-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="138bd-218">Request</span></span>
<span data-ttu-id="138bd-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="138bd-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1123

{
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="138bd-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="138bd-220">Response</span></span>
<span data-ttu-id="138bd-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="138bd-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1289

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





