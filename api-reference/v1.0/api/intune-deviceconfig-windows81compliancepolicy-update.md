---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68e74069a00748a6e94f096dc483061be9ce4b78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987255"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="0de28-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0de28-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="0de28-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0de28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0de28-105">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0de28-105">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0de28-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0de28-106">Prerequisites</span></span>
<span data-ttu-id="0de28-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de28-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0de28-109">Permission type</span></span>|<span data-ttu-id="0de28-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0de28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0de28-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0de28-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0de28-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de28-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0de28-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0de28-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0de28-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de28-114">Not supported.</span></span>|
|<span data-ttu-id="0de28-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0de28-115">Application</span></span>|<span data-ttu-id="0de28-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de28-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0de28-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0de28-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0de28-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0de28-118">Request headers</span></span>
|<span data-ttu-id="0de28-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0de28-119">Header</span></span>|<span data-ttu-id="0de28-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0de28-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0de28-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0de28-121">Authorization</span></span>|<span data-ttu-id="0de28-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de28-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0de28-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0de28-123">Accept</span></span>|<span data-ttu-id="0de28-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0de28-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0de28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0de28-125">Request body</span></span>
<span data-ttu-id="0de28-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0de28-126">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="0de28-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0de28-127">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="0de28-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0de28-128">Property</span></span>|<span data-ttu-id="0de28-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="0de28-129">Type</span></span>|<span data-ttu-id="0de28-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="0de28-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de28-131">id</span><span class="sxs-lookup"><span data-stu-id="0de28-131">id</span></span>|<span data-ttu-id="0de28-132">String</span><span class="sxs-lookup"><span data-stu-id="0de28-132">String</span></span>|<span data-ttu-id="0de28-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0de28-133">Key of the entity.</span></span> <span data-ttu-id="0de28-134">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0de28-135">createdDateTime</span></span>|<span data-ttu-id="0de28-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0de28-136">DateTimeOffset</span></span>|<span data-ttu-id="0de28-137">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0de28-137">DateTime the object was created.</span></span> <span data-ttu-id="0de28-138">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-139">description</span><span class="sxs-lookup"><span data-stu-id="0de28-139">description</span></span>|<span data-ttu-id="0de28-140">String</span><span class="sxs-lookup"><span data-stu-id="0de28-140">String</span></span>|<span data-ttu-id="0de28-141">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0de28-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0de28-142">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0de28-143">lastModifiedDateTime</span></span>|<span data-ttu-id="0de28-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0de28-144">DateTimeOffset</span></span>|<span data-ttu-id="0de28-145">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0de28-145">DateTime the object was last modified.</span></span> <span data-ttu-id="0de28-146">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0de28-147">displayName</span></span>|<span data-ttu-id="0de28-148">String</span><span class="sxs-lookup"><span data-stu-id="0de28-148">String</span></span>|<span data-ttu-id="0de28-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0de28-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0de28-150">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-151">version</span><span class="sxs-lookup"><span data-stu-id="0de28-151">version</span></span>|<span data-ttu-id="0de28-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-152">Int32</span></span>|<span data-ttu-id="0de28-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0de28-153">Version of the device configuration.</span></span> <span data-ttu-id="0de28-154">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0de28-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0de28-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0de28-155">passwordRequired</span></span>|<span data-ttu-id="0de28-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="0de28-156">Boolean</span></span>|<span data-ttu-id="0de28-157">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="0de28-157">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="0de28-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0de28-158">passwordBlockSimple</span></span>|<span data-ttu-id="0de28-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="0de28-159">Boolean</span></span>|<span data-ttu-id="0de28-160">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0de28-160">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="0de28-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0de28-161">passwordExpirationDays</span></span>|<span data-ttu-id="0de28-162">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-162">Int32</span></span>|<span data-ttu-id="0de28-163">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="0de28-163">Password expiration in days.</span></span>|
|<span data-ttu-id="0de28-164">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0de28-164">passwordMinimumLength</span></span>|<span data-ttu-id="0de28-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-165">Int32</span></span>|<span data-ttu-id="0de28-166">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0de28-166">The minimum password length.</span></span>|
|<span data-ttu-id="0de28-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0de28-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0de28-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-168">Int32</span></span>|<span data-ttu-id="0de28-169">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0de28-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0de28-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0de28-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0de28-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-171">Int32</span></span>|<span data-ttu-id="0de28-172">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="0de28-172">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0de28-173">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0de28-173">passwordRequiredType</span></span>|[<span data-ttu-id="0de28-174">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0de28-174">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0de28-175">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="0de28-175">The required password type.</span></span> <span data-ttu-id="0de28-176">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0de28-176">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0de28-177">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0de28-177">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0de28-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0de28-178">Int32</span></span>|<span data-ttu-id="0de28-179">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="0de28-179">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0de28-180">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="0de28-180">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0de28-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0de28-181">osMinimumVersion</span></span>|<span data-ttu-id="0de28-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0de28-182">String</span></span>|<span data-ttu-id="0de28-183">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0de28-183">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0de28-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0de28-184">osMaximumVersion</span></span>|<span data-ttu-id="0de28-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0de28-185">String</span></span>|<span data-ttu-id="0de28-186">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0de28-186">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0de28-187">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0de28-187">storageRequireEncryption</span></span>|<span data-ttu-id="0de28-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="0de28-188">Boolean</span></span>|<span data-ttu-id="0de28-189">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0de28-189">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="0de28-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de28-190">Response</span></span>
<span data-ttu-id="0de28-191">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0de28-191">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0de28-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0de28-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="0de28-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de28-193">Request</span></span>
<span data-ttu-id="0de28-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de28-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0de28-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de28-195">Response</span></span>
<span data-ttu-id="0de28-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de28-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



