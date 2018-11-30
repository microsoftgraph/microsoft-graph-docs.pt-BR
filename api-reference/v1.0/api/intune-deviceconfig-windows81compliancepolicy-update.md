---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
ms.openlocfilehash: 52e76e1be627633f6bba0a78c451afb8b184d265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005803"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="be46c-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="be46c-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="be46c-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="be46c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be46c-105">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be46c-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be46c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="be46c-106">Prerequisites</span></span>
<span data-ttu-id="be46c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be46c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be46c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be46c-109">Permission type</span></span>|<span data-ttu-id="be46c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="be46c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be46c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be46c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be46c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be46c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be46c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be46c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be46c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be46c-114">Not supported.</span></span>|
|<span data-ttu-id="be46c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be46c-115">Application</span></span>|<span data-ttu-id="be46c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be46c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be46c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be46c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="be46c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be46c-118">Request headers</span></span>
|<span data-ttu-id="be46c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be46c-119">Header</span></span>|<span data-ttu-id="be46c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="be46c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be46c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be46c-121">Authorization</span></span>|<span data-ttu-id="be46c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be46c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be46c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="be46c-123">Accept</span></span>|<span data-ttu-id="be46c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be46c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be46c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be46c-125">Request body</span></span>
<span data-ttu-id="be46c-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be46c-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="be46c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="be46c-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="be46c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be46c-128">Property</span></span>|<span data-ttu-id="be46c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="be46c-129">Type</span></span>|<span data-ttu-id="be46c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="be46c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be46c-131">id</span><span class="sxs-lookup"><span data-stu-id="be46c-131">id</span></span>|<span data-ttu-id="be46c-132">String</span><span class="sxs-lookup"><span data-stu-id="be46c-132">String</span></span>|<span data-ttu-id="be46c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="be46c-133">Key of the entity.</span></span> <span data-ttu-id="be46c-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be46c-135">createdDateTime</span></span>|<span data-ttu-id="be46c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be46c-136">DateTimeOffset</span></span>|<span data-ttu-id="be46c-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="be46c-137">DateTime the object was created.</span></span> <span data-ttu-id="be46c-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-139">description</span><span class="sxs-lookup"><span data-stu-id="be46c-139">description</span></span>|<span data-ttu-id="be46c-140">String</span><span class="sxs-lookup"><span data-stu-id="be46c-140">String</span></span>|<span data-ttu-id="be46c-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be46c-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be46c-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be46c-143">lastModifiedDateTime</span></span>|<span data-ttu-id="be46c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be46c-144">DateTimeOffset</span></span>|<span data-ttu-id="be46c-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="be46c-145">DateTime the object was last modified.</span></span> <span data-ttu-id="be46c-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="be46c-147">displayName</span></span>|<span data-ttu-id="be46c-148">String</span><span class="sxs-lookup"><span data-stu-id="be46c-148">String</span></span>|<span data-ttu-id="be46c-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be46c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be46c-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-151">version</span><span class="sxs-lookup"><span data-stu-id="be46c-151">version</span></span>|<span data-ttu-id="be46c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-152">Int32</span></span>|<span data-ttu-id="be46c-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="be46c-153">Version of the device configuration.</span></span> <span data-ttu-id="be46c-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="be46c-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="be46c-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="be46c-155">passwordRequired</span></span>|<span data-ttu-id="be46c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="be46c-156">Boolean</span></span>|<span data-ttu-id="be46c-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="be46c-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="be46c-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="be46c-158">passwordBlockSimple</span></span>|<span data-ttu-id="be46c-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="be46c-159">Boolean</span></span>|<span data-ttu-id="be46c-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="be46c-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="be46c-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="be46c-161">passwordExpirationDays</span></span>|<span data-ttu-id="be46c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-162">Int32</span></span>|<span data-ttu-id="be46c-163">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="be46c-163">Password expiration in days.</span></span>|
|<span data-ttu-id="be46c-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="be46c-164">passwordMinimumLength</span></span>|<span data-ttu-id="be46c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-165">Int32</span></span>|<span data-ttu-id="be46c-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="be46c-166">The minimum password length.</span></span>|
|<span data-ttu-id="be46c-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="be46c-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="be46c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-168">Int32</span></span>|<span data-ttu-id="be46c-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="be46c-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="be46c-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="be46c-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="be46c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-171">Int32</span></span>|<span data-ttu-id="be46c-172">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="be46c-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="be46c-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="be46c-173">passwordRequiredType</span></span>|[<span data-ttu-id="be46c-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="be46c-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="be46c-175">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="be46c-175">The required password type.</span></span> <span data-ttu-id="be46c-176">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="be46c-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="be46c-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="be46c-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="be46c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="be46c-178">Int32</span></span>|<span data-ttu-id="be46c-179">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="be46c-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="be46c-180">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="be46c-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="be46c-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="be46c-181">osMinimumVersion</span></span>|<span data-ttu-id="be46c-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be46c-182">String</span></span>|<span data-ttu-id="be46c-183">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="be46c-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="be46c-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="be46c-184">osMaximumVersion</span></span>|<span data-ttu-id="be46c-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="be46c-185">String</span></span>|<span data-ttu-id="be46c-186">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="be46c-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="be46c-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="be46c-187">storageRequireEncryption</span></span>|<span data-ttu-id="be46c-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="be46c-188">Boolean</span></span>|<span data-ttu-id="be46c-189">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="be46c-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="be46c-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="be46c-190">Response</span></span>
<span data-ttu-id="be46c-191">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be46c-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be46c-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be46c-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="be46c-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be46c-193">Request</span></span>
<span data-ttu-id="be46c-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be46c-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="be46c-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="be46c-195">Response</span></span>
<span data-ttu-id="be46c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be46c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
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



