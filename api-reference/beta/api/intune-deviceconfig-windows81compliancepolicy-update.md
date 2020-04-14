---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c46a5f12320f8e6eea80fda6dff54a2b8fb6e44b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430511"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="34b2f-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="34b2f-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="34b2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34b2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34b2f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34b2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34b2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34b2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34b2f-107">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34b2f-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34b2f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34b2f-108">Prerequisites</span></span>
<span data-ttu-id="34b2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34b2f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34b2f-111">Permission type</span></span>|<span data-ttu-id="34b2f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34b2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34b2f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34b2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34b2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34b2f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34b2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34b2f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34b2f-116">Not supported.</span></span>|
|<span data-ttu-id="34b2f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34b2f-117">Application</span></span>|<span data-ttu-id="34b2f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34b2f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34b2f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34b2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="34b2f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34b2f-120">Request headers</span></span>
|<span data-ttu-id="34b2f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34b2f-121">Header</span></span>|<span data-ttu-id="34b2f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="34b2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34b2f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34b2f-123">Authorization</span></span>|<span data-ttu-id="34b2f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34b2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34b2f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34b2f-125">Accept</span></span>|<span data-ttu-id="34b2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34b2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34b2f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34b2f-127">Request body</span></span>
<span data-ttu-id="34b2f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34b2f-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="34b2f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34b2f-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="34b2f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34b2f-130">Property</span></span>|<span data-ttu-id="34b2f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="34b2f-131">Type</span></span>|<span data-ttu-id="34b2f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="34b2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34b2f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34b2f-133">roleScopeTagIds</span></span>|<span data-ttu-id="34b2f-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="34b2f-134">String collection</span></span>|<span data-ttu-id="34b2f-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="34b2f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34b2f-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-137">id</span><span class="sxs-lookup"><span data-stu-id="34b2f-137">id</span></span>|<span data-ttu-id="34b2f-138">String</span><span class="sxs-lookup"><span data-stu-id="34b2f-138">String</span></span>|<span data-ttu-id="34b2f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34b2f-139">Key of the entity.</span></span> <span data-ttu-id="34b2f-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34b2f-141">createdDateTime</span></span>|<span data-ttu-id="34b2f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b2f-142">DateTimeOffset</span></span>|<span data-ttu-id="34b2f-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="34b2f-143">DateTime the object was created.</span></span> <span data-ttu-id="34b2f-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-145">description</span><span class="sxs-lookup"><span data-stu-id="34b2f-145">description</span></span>|<span data-ttu-id="34b2f-146">String</span><span class="sxs-lookup"><span data-stu-id="34b2f-146">String</span></span>|<span data-ttu-id="34b2f-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34b2f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34b2f-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34b2f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="34b2f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b2f-150">DateTimeOffset</span></span>|<span data-ttu-id="34b2f-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="34b2f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="34b2f-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="34b2f-153">displayName</span></span>|<span data-ttu-id="34b2f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b2f-154">String</span></span>|<span data-ttu-id="34b2f-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34b2f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34b2f-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-157">version</span><span class="sxs-lookup"><span data-stu-id="34b2f-157">version</span></span>|<span data-ttu-id="34b2f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-158">Int32</span></span>|<span data-ttu-id="34b2f-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34b2f-159">Version of the device configuration.</span></span> <span data-ttu-id="34b2f-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="34b2f-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="34b2f-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="34b2f-161">passwordRequired</span></span>|<span data-ttu-id="34b2f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="34b2f-162">Boolean</span></span>|<span data-ttu-id="34b2f-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="34b2f-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="34b2f-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="34b2f-164">passwordBlockSimple</span></span>|<span data-ttu-id="34b2f-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="34b2f-165">Boolean</span></span>|<span data-ttu-id="34b2f-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="34b2f-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="34b2f-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34b2f-167">passwordExpirationDays</span></span>|<span data-ttu-id="34b2f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-168">Int32</span></span>|<span data-ttu-id="34b2f-169">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="34b2f-169">Password expiration in days.</span></span>|
|<span data-ttu-id="34b2f-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34b2f-170">passwordMinimumLength</span></span>|<span data-ttu-id="34b2f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-171">Int32</span></span>|<span data-ttu-id="34b2f-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="34b2f-172">The minimum password length.</span></span>|
|<span data-ttu-id="34b2f-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="34b2f-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="34b2f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-174">Int32</span></span>|<span data-ttu-id="34b2f-175">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="34b2f-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="34b2f-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="34b2f-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="34b2f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-177">Int32</span></span>|<span data-ttu-id="34b2f-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="34b2f-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="34b2f-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34b2f-179">passwordRequiredType</span></span>|[<span data-ttu-id="34b2f-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34b2f-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="34b2f-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="34b2f-181">The required password type.</span></span> <span data-ttu-id="34b2f-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="34b2f-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="34b2f-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34b2f-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34b2f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="34b2f-184">Int32</span></span>|<span data-ttu-id="34b2f-185">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="34b2f-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="34b2f-186">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="34b2f-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="34b2f-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="34b2f-187">osMinimumVersion</span></span>|<span data-ttu-id="34b2f-188">String</span><span class="sxs-lookup"><span data-stu-id="34b2f-188">String</span></span>|<span data-ttu-id="34b2f-189">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="34b2f-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="34b2f-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="34b2f-190">osMaximumVersion</span></span>|<span data-ttu-id="34b2f-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34b2f-191">String</span></span>|<span data-ttu-id="34b2f-192">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="34b2f-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="34b2f-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="34b2f-193">storageRequireEncryption</span></span>|<span data-ttu-id="34b2f-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="34b2f-194">Boolean</span></span>|<span data-ttu-id="34b2f-195">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="34b2f-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="34b2f-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b2f-196">Response</span></span>
<span data-ttu-id="34b2f-197">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34b2f-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34b2f-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34b2f-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="34b2f-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34b2f-199">Request</span></span>
<span data-ttu-id="34b2f-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34b2f-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 664

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="34b2f-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="34b2f-201">Response</span></span>
<span data-ttu-id="34b2f-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34b2f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



