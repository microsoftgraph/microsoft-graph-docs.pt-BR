---
title: Criar windowsPhone81CompliancePolicy
description: Cria um novo objeto windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6ba95411610b8cc71917e344ad9d1d41b402be16
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812030"
---
# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="e7d3c-103">Criar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e7d3c-103">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="e7d3c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7d3c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7d3c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7d3c-107">Cria um novo objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e7d3c-107">Create a new [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7d3c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7d3c-108">Prerequisites</span></span>
<span data-ttu-id="e7d3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d3c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7d3c-111">Permission type</span></span>|<span data-ttu-id="e7d3c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d3c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d3c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d3c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7d3c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-116">Not supported.</span></span>|
|<span data-ttu-id="e7d3c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7d3c-117">Application</span></span>|<span data-ttu-id="e7d3c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d3c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7d3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="e7d3c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d3c-120">Request headers</span></span>
|<span data-ttu-id="e7d3c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7d3c-121">Header</span></span>|<span data-ttu-id="e7d3c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e7d3c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d3c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7d3c-123">Authorization</span></span>|<span data-ttu-id="e7d3c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d3c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7d3c-125">Accept</span></span>|<span data-ttu-id="e7d3c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d3c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d3c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d3c-127">Request body</span></span>
<span data-ttu-id="e7d3c-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-128">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="e7d3c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsPhone81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-129">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="e7d3c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7d3c-130">Property</span></span>|<span data-ttu-id="e7d3c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7d3c-131">Type</span></span>|<span data-ttu-id="e7d3c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7d3c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d3c-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7d3c-133">roleScopeTagIds</span></span>|<span data-ttu-id="e7d3c-134">String collection</span><span class="sxs-lookup"><span data-stu-id="e7d3c-134">String collection</span></span>|<span data-ttu-id="e7d3c-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7d3c-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-137">id</span><span class="sxs-lookup"><span data-stu-id="e7d3c-137">id</span></span>|<span data-ttu-id="e7d3c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d3c-138">String</span></span>|<span data-ttu-id="e7d3c-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-139">Key of the entity.</span></span> <span data-ttu-id="e7d3c-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d3c-141">createdDateTime</span></span>|<span data-ttu-id="e7d3c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d3c-142">DateTimeOffset</span></span>|<span data-ttu-id="e7d3c-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-143">DateTime the object was created.</span></span> <span data-ttu-id="e7d3c-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-145">description</span><span class="sxs-lookup"><span data-stu-id="e7d3c-145">description</span></span>|<span data-ttu-id="e7d3c-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d3c-146">String</span></span>|<span data-ttu-id="e7d3c-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7d3c-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d3c-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e7d3c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d3c-150">DateTimeOffset</span></span>|<span data-ttu-id="e7d3c-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-151">DateTime the object was last modified.</span></span> <span data-ttu-id="e7d3c-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-153">displayName</span><span class="sxs-lookup"><span data-stu-id="e7d3c-153">displayName</span></span>|<span data-ttu-id="e7d3c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d3c-154">String</span></span>|<span data-ttu-id="e7d3c-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7d3c-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-157">version</span><span class="sxs-lookup"><span data-stu-id="e7d3c-157">version</span></span>|<span data-ttu-id="e7d3c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-158">Int32</span></span>|<span data-ttu-id="e7d3c-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-159">Version of the device configuration.</span></span> <span data-ttu-id="e7d3c-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e7d3c-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="e7d3c-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e7d3c-161">passwordBlockSimple</span></span>|<span data-ttu-id="e7d3c-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7d3c-162">Boolean</span></span>|<span data-ttu-id="e7d3c-163">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="e7d3c-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e7d3c-164">passwordExpirationDays</span></span>|<span data-ttu-id="e7d3c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-165">Int32</span></span>|<span data-ttu-id="e7d3c-166">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e7d3c-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e7d3c-167">passwordMinimumLength</span></span>|<span data-ttu-id="e7d3c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-168">Int32</span></span>|<span data-ttu-id="e7d3c-169">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e7d3c-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e7d3c-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e7d3c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-171">Int32</span></span>|<span data-ttu-id="e7d3c-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="e7d3c-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e7d3c-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e7d3c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-174">Int32</span></span>|<span data-ttu-id="e7d3c-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="e7d3c-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e7d3c-176">passwordRequiredType</span></span>|[<span data-ttu-id="e7d3c-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e7d3c-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e7d3c-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-178">The required password type.</span></span> <span data-ttu-id="e7d3c-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e7d3c-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e7d3c-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e7d3c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d3c-181">Int32</span></span>|<span data-ttu-id="e7d3c-182">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-182">Number of previous passwords to block.</span></span> <span data-ttu-id="e7d3c-183">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e7d3c-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e7d3c-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e7d3c-184">passwordRequired</span></span>|<span data-ttu-id="e7d3c-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7d3c-185">Boolean</span></span>|<span data-ttu-id="e7d3c-186">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e7d3c-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e7d3c-187">osMinimumVersion</span></span>|<span data-ttu-id="e7d3c-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d3c-188">String</span></span>|<span data-ttu-id="e7d3c-189">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="e7d3c-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e7d3c-190">osMaximumVersion</span></span>|<span data-ttu-id="e7d3c-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7d3c-191">String</span></span>|<span data-ttu-id="e7d3c-192">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="e7d3c-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="e7d3c-193">storageRequireEncryption</span></span>|<span data-ttu-id="e7d3c-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7d3c-194">Boolean</span></span>|<span data-ttu-id="e7d3c-195">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="e7d3c-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d3c-196">Response</span></span>
<span data-ttu-id="e7d3c-197">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-197">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7d3c-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7d3c-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7d3c-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7d3c-199">Request</span></span>
<span data-ttu-id="e7d3c-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 733

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="e7d3c-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7d3c-201">Response</span></span>
<span data-ttu-id="e7d3c-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7d3c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





