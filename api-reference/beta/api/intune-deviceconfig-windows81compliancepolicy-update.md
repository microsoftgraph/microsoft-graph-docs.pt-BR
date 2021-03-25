---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 577b216801c67275067211100d03fb9ece1af3ab
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151064"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="084a5-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="084a5-103">Update windows81CompliancePolicy</span></span>

<span data-ttu-id="084a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="084a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="084a5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="084a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="084a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="084a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="084a5-107">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="084a5-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="084a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="084a5-108">Prerequisites</span></span>
<span data-ttu-id="084a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="084a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="084a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="084a5-111">Permission type</span></span>|<span data-ttu-id="084a5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="084a5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="084a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="084a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="084a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="084a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="084a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="084a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="084a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="084a5-116">Not supported.</span></span>|
|<span data-ttu-id="084a5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="084a5-117">Application</span></span>|<span data-ttu-id="084a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="084a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="084a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="084a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="084a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="084a5-120">Request headers</span></span>
|<span data-ttu-id="084a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="084a5-121">Header</span></span>|<span data-ttu-id="084a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="084a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="084a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="084a5-123">Authorization</span></span>|<span data-ttu-id="084a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="084a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="084a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="084a5-125">Accept</span></span>|<span data-ttu-id="084a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="084a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="084a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="084a5-127">Request body</span></span>
<span data-ttu-id="084a5-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="084a5-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="084a5-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="084a5-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="084a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="084a5-130">Property</span></span>|<span data-ttu-id="084a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="084a5-131">Type</span></span>|<span data-ttu-id="084a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="084a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="084a5-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="084a5-133">roleScopeTagIds</span></span>|<span data-ttu-id="084a5-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-134">String collection</span></span>|<span data-ttu-id="084a5-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="084a5-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="084a5-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-137">id</span><span class="sxs-lookup"><span data-stu-id="084a5-137">id</span></span>|<span data-ttu-id="084a5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-138">String</span></span>|<span data-ttu-id="084a5-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="084a5-139">Key of the entity.</span></span> <span data-ttu-id="084a5-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="084a5-141">createdDateTime</span></span>|<span data-ttu-id="084a5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="084a5-142">DateTimeOffset</span></span>|<span data-ttu-id="084a5-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="084a5-143">DateTime the object was created.</span></span> <span data-ttu-id="084a5-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-145">descrição</span><span class="sxs-lookup"><span data-stu-id="084a5-145">description</span></span>|<span data-ttu-id="084a5-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-146">String</span></span>|<span data-ttu-id="084a5-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="084a5-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="084a5-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="084a5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="084a5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="084a5-150">DateTimeOffset</span></span>|<span data-ttu-id="084a5-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="084a5-151">DateTime the object was last modified.</span></span> <span data-ttu-id="084a5-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-153">displayName</span><span class="sxs-lookup"><span data-stu-id="084a5-153">displayName</span></span>|<span data-ttu-id="084a5-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-154">String</span></span>|<span data-ttu-id="084a5-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="084a5-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="084a5-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-157">version</span><span class="sxs-lookup"><span data-stu-id="084a5-157">version</span></span>|<span data-ttu-id="084a5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-158">Int32</span></span>|<span data-ttu-id="084a5-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="084a5-159">Version of the device configuration.</span></span> <span data-ttu-id="084a5-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="084a5-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="084a5-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="084a5-161">passwordRequired</span></span>|<span data-ttu-id="084a5-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="084a5-162">Boolean</span></span>|<span data-ttu-id="084a5-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="084a5-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="084a5-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="084a5-164">passwordBlockSimple</span></span>|<span data-ttu-id="084a5-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="084a5-165">Boolean</span></span>|<span data-ttu-id="084a5-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="084a5-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="084a5-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="084a5-167">passwordExpirationDays</span></span>|<span data-ttu-id="084a5-168">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-168">Int32</span></span>|<span data-ttu-id="084a5-169">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="084a5-169">Password expiration in days.</span></span>|
|<span data-ttu-id="084a5-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="084a5-170">passwordMinimumLength</span></span>|<span data-ttu-id="084a5-171">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-171">Int32</span></span>|<span data-ttu-id="084a5-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="084a5-172">The minimum password length.</span></span>|
|<span data-ttu-id="084a5-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="084a5-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="084a5-174">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-174">Int32</span></span>|<span data-ttu-id="084a5-175">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="084a5-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="084a5-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="084a5-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="084a5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-177">Int32</span></span>|<span data-ttu-id="084a5-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="084a5-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="084a5-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="084a5-179">passwordRequiredType</span></span>|[<span data-ttu-id="084a5-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="084a5-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="084a5-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="084a5-181">The required password type.</span></span> <span data-ttu-id="084a5-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="084a5-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="084a5-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="084a5-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="084a5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="084a5-184">Int32</span></span>|<span data-ttu-id="084a5-185">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="084a5-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="084a5-186">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="084a5-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="084a5-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="084a5-187">osMinimumVersion</span></span>|<span data-ttu-id="084a5-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-188">String</span></span>|<span data-ttu-id="084a5-189">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="084a5-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="084a5-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="084a5-190">osMaximumVersion</span></span>|<span data-ttu-id="084a5-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="084a5-191">String</span></span>|<span data-ttu-id="084a5-192">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="084a5-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="084a5-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="084a5-193">storageRequireEncryption</span></span>|<span data-ttu-id="084a5-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="084a5-194">Boolean</span></span>|<span data-ttu-id="084a5-195">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="084a5-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="084a5-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="084a5-196">Response</span></span>
<span data-ttu-id="084a5-197">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="084a5-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="084a5-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="084a5-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="084a5-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="084a5-199">Request</span></span>
<span data-ttu-id="084a5-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="084a5-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="084a5-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="084a5-201">Response</span></span>
<span data-ttu-id="084a5-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="084a5-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




