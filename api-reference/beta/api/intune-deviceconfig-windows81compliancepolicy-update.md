---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a84642fd7df4f64f7888422bc88557c7be603beb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314228"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="9ff91-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9ff91-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="9ff91-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ff91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff91-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ff91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff91-106">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff91-106">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff91-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ff91-107">Prerequisites</span></span>
<span data-ttu-id="9ff91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff91-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ff91-110">Permission type</span></span>|<span data-ttu-id="9ff91-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ff91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff91-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ff91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff91-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff91-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ff91-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ff91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff91-115">Not supported.</span></span>|
|<span data-ttu-id="9ff91-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ff91-116">Application</span></span>|<span data-ttu-id="9ff91-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff91-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff91-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="9ff91-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff91-119">Request headers</span></span>
|<span data-ttu-id="9ff91-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ff91-120">Header</span></span>|<span data-ttu-id="9ff91-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9ff91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff91-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ff91-122">Authorization</span></span>|<span data-ttu-id="9ff91-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ff91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff91-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ff91-124">Accept</span></span>|<span data-ttu-id="9ff91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff91-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff91-126">Request body</span></span>
<span data-ttu-id="9ff91-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff91-127">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="9ff91-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9ff91-128">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="9ff91-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ff91-129">Property</span></span>|<span data-ttu-id="9ff91-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ff91-130">Type</span></span>|<span data-ttu-id="9ff91-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ff91-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff91-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ff91-132">roleScopeTagIds</span></span>|<span data-ttu-id="9ff91-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ff91-133">String collection</span></span>|<span data-ttu-id="9ff91-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9ff91-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ff91-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-136">id</span><span class="sxs-lookup"><span data-stu-id="9ff91-136">id</span></span>|<span data-ttu-id="9ff91-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ff91-137">String</span></span>|<span data-ttu-id="9ff91-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ff91-138">Key of the entity.</span></span> <span data-ttu-id="9ff91-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff91-140">createdDateTime</span></span>|<span data-ttu-id="9ff91-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff91-141">DateTimeOffset</span></span>|<span data-ttu-id="9ff91-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ff91-142">DateTime the object was created.</span></span> <span data-ttu-id="9ff91-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-144">descrição</span><span class="sxs-lookup"><span data-stu-id="9ff91-144">description</span></span>|<span data-ttu-id="9ff91-145">String</span><span class="sxs-lookup"><span data-stu-id="9ff91-145">String</span></span>|<span data-ttu-id="9ff91-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff91-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ff91-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff91-148">lastModifiedDateTime</span></span>|<span data-ttu-id="9ff91-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff91-149">DateTimeOffset</span></span>|<span data-ttu-id="9ff91-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ff91-150">DateTime the object was last modified.</span></span> <span data-ttu-id="9ff91-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-152">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff91-152">displayName</span></span>|<span data-ttu-id="9ff91-153">String</span><span class="sxs-lookup"><span data-stu-id="9ff91-153">String</span></span>|<span data-ttu-id="9ff91-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff91-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ff91-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-156">version</span><span class="sxs-lookup"><span data-stu-id="9ff91-156">version</span></span>|<span data-ttu-id="9ff91-157">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-157">Int32</span></span>|<span data-ttu-id="9ff91-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff91-158">Version of the device configuration.</span></span> <span data-ttu-id="9ff91-159">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9ff91-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="9ff91-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9ff91-160">passwordRequired</span></span>|<span data-ttu-id="9ff91-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ff91-161">Boolean</span></span>|<span data-ttu-id="9ff91-162">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="9ff91-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="9ff91-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9ff91-163">passwordBlockSimple</span></span>|<span data-ttu-id="9ff91-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ff91-164">Boolean</span></span>|<span data-ttu-id="9ff91-165">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9ff91-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="9ff91-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9ff91-166">passwordExpirationDays</span></span>|<span data-ttu-id="9ff91-167">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-167">Int32</span></span>|<span data-ttu-id="9ff91-168">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="9ff91-168">Password expiration in days.</span></span>|
|<span data-ttu-id="9ff91-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9ff91-169">passwordMinimumLength</span></span>|<span data-ttu-id="9ff91-170">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-170">Int32</span></span>|<span data-ttu-id="9ff91-171">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="9ff91-171">The minimum password length.</span></span>|
|<span data-ttu-id="9ff91-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9ff91-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9ff91-173">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-173">Int32</span></span>|<span data-ttu-id="9ff91-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="9ff91-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="9ff91-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9ff91-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9ff91-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-176">Int32</span></span>|<span data-ttu-id="9ff91-177">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="9ff91-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9ff91-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9ff91-178">passwordRequiredType</span></span>|[<span data-ttu-id="9ff91-179">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9ff91-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9ff91-180">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="9ff91-180">The required password type.</span></span> <span data-ttu-id="9ff91-181">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9ff91-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9ff91-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9ff91-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9ff91-183">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff91-183">Int32</span></span>|<span data-ttu-id="9ff91-184">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="9ff91-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9ff91-185">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="9ff91-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9ff91-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="9ff91-186">osMinimumVersion</span></span>|<span data-ttu-id="9ff91-187">String</span><span class="sxs-lookup"><span data-stu-id="9ff91-187">String</span></span>|<span data-ttu-id="9ff91-188">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9ff91-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9ff91-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="9ff91-189">osMaximumVersion</span></span>|<span data-ttu-id="9ff91-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ff91-190">String</span></span>|<span data-ttu-id="9ff91-191">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9ff91-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="9ff91-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9ff91-192">storageRequireEncryption</span></span>|<span data-ttu-id="9ff91-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ff91-193">Boolean</span></span>|<span data-ttu-id="9ff91-194">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9ff91-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="9ff91-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff91-195">Response</span></span>
<span data-ttu-id="9ff91-196">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff91-196">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff91-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ff91-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff91-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff91-198">Request</span></span>
<span data-ttu-id="9ff91-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ff91-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ff91-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff91-200">Response</span></span>
<span data-ttu-id="9ff91-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ff91-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






