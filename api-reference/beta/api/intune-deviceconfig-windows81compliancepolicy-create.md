---
title: Criar windows81CompliancePolicy
description: Cria um novo objeto windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bee3e80b08b19009f61fa82ba334dcf962c993c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822600"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="9c85b-103">Criar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9c85b-103">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="9c85b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c85b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c85b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c85b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c85b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c85b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c85b-107">Cria um novo objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9c85b-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c85b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c85b-108">Prerequisites</span></span>
<span data-ttu-id="9c85b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c85b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c85b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c85b-111">Permission type</span></span>|<span data-ttu-id="9c85b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c85b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c85b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c85b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c85b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c85b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c85b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c85b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c85b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c85b-116">Not supported.</span></span>|
|<span data-ttu-id="9c85b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c85b-117">Application</span></span>|<span data-ttu-id="9c85b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c85b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c85b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c85b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9c85b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c85b-120">Request headers</span></span>
|<span data-ttu-id="9c85b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c85b-121">Header</span></span>|<span data-ttu-id="9c85b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9c85b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c85b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c85b-123">Authorization</span></span>|<span data-ttu-id="9c85b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c85b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c85b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c85b-125">Accept</span></span>|<span data-ttu-id="9c85b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c85b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c85b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c85b-127">Request body</span></span>
<span data-ttu-id="9c85b-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9c85b-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="9c85b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="9c85b-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="9c85b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c85b-130">Property</span></span>|<span data-ttu-id="9c85b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c85b-131">Type</span></span>|<span data-ttu-id="9c85b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c85b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c85b-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c85b-133">roleScopeTagIds</span></span>|<span data-ttu-id="9c85b-134">String collection</span><span class="sxs-lookup"><span data-stu-id="9c85b-134">String collection</span></span>|<span data-ttu-id="9c85b-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9c85b-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c85b-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-137">id</span><span class="sxs-lookup"><span data-stu-id="9c85b-137">id</span></span>|<span data-ttu-id="9c85b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c85b-138">String</span></span>|<span data-ttu-id="9c85b-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9c85b-139">Key of the entity.</span></span> <span data-ttu-id="9c85b-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c85b-141">createdDateTime</span></span>|<span data-ttu-id="9c85b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c85b-142">DateTimeOffset</span></span>|<span data-ttu-id="9c85b-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9c85b-143">DateTime the object was created.</span></span> <span data-ttu-id="9c85b-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-145">description</span><span class="sxs-lookup"><span data-stu-id="9c85b-145">description</span></span>|<span data-ttu-id="9c85b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c85b-146">String</span></span>|<span data-ttu-id="9c85b-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c85b-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c85b-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c85b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="9c85b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c85b-150">DateTimeOffset</span></span>|<span data-ttu-id="9c85b-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9c85b-151">DateTime the object was last modified.</span></span> <span data-ttu-id="9c85b-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="9c85b-153">displayName</span></span>|<span data-ttu-id="9c85b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c85b-154">String</span></span>|<span data-ttu-id="9c85b-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c85b-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c85b-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-157">version</span><span class="sxs-lookup"><span data-stu-id="9c85b-157">version</span></span>|<span data-ttu-id="9c85b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-158">Int32</span></span>|<span data-ttu-id="9c85b-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c85b-159">Version of the device configuration.</span></span> <span data-ttu-id="9c85b-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9c85b-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9c85b-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9c85b-161">passwordRequired</span></span>|<span data-ttu-id="9c85b-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c85b-162">Boolean</span></span>|<span data-ttu-id="9c85b-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="9c85b-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="9c85b-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9c85b-164">passwordBlockSimple</span></span>|<span data-ttu-id="9c85b-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c85b-165">Boolean</span></span>|<span data-ttu-id="9c85b-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9c85b-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="9c85b-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9c85b-167">passwordExpirationDays</span></span>|<span data-ttu-id="9c85b-168">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-168">Int32</span></span>|<span data-ttu-id="9c85b-169">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="9c85b-169">Password expiration in days.</span></span>|
|<span data-ttu-id="9c85b-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9c85b-170">passwordMinimumLength</span></span>|<span data-ttu-id="9c85b-171">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-171">Int32</span></span>|<span data-ttu-id="9c85b-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="9c85b-172">The minimum password length.</span></span>|
|<span data-ttu-id="9c85b-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9c85b-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9c85b-174">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-174">Int32</span></span>|<span data-ttu-id="9c85b-175">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="9c85b-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9c85b-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9c85b-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9c85b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-177">Int32</span></span>|<span data-ttu-id="9c85b-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="9c85b-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9c85b-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9c85b-179">passwordRequiredType</span></span>|[<span data-ttu-id="9c85b-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9c85b-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9c85b-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="9c85b-181">The required password type.</span></span> <span data-ttu-id="9c85b-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9c85b-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9c85b-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9c85b-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9c85b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9c85b-184">Int32</span></span>|<span data-ttu-id="9c85b-185">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="9c85b-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9c85b-186">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="9c85b-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9c85b-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9c85b-187">osMinimumVersion</span></span>|<span data-ttu-id="9c85b-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c85b-188">String</span></span>|<span data-ttu-id="9c85b-189">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9c85b-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9c85b-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9c85b-190">osMaximumVersion</span></span>|<span data-ttu-id="9c85b-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9c85b-191">String</span></span>|<span data-ttu-id="9c85b-192">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9c85b-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9c85b-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9c85b-193">storageRequireEncryption</span></span>|<span data-ttu-id="9c85b-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="9c85b-194">Boolean</span></span>|<span data-ttu-id="9c85b-195">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9c85b-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="9c85b-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c85b-196">Response</span></span>
<span data-ttu-id="9c85b-197">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c85b-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c85b-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c85b-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c85b-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c85b-199">Request</span></span>
<span data-ttu-id="9c85b-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c85b-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="9c85b-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c85b-201">Response</span></span>
<span data-ttu-id="9c85b-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c85b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 836

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```





