---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb60f25a1840dae55458266982c6a0be69c176ca
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187195"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="0a1bd-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0a1bd-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="0a1bd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a1bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a1bd-106">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-106">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a1bd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a1bd-107">Prerequisites</span></span>
<span data-ttu-id="0a1bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a1bd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a1bd-110">Permission type</span></span>|<span data-ttu-id="0a1bd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a1bd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1bd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a1bd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a1bd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-115">Not supported.</span></span>|
|<span data-ttu-id="0a1bd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a1bd-116">Application</span></span>|<span data-ttu-id="0a1bd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a1bd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a1bd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a1bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="0a1bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-119">Request headers</span></span>
|<span data-ttu-id="0a1bd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a1bd-120">Header</span></span>|<span data-ttu-id="0a1bd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0a1bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a1bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a1bd-122">Authorization</span></span>|<span data-ttu-id="0a1bd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a1bd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a1bd-124">Accept</span></span>|<span data-ttu-id="0a1bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a1bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a1bd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-126">Request body</span></span>
<span data-ttu-id="0a1bd-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-127">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="0a1bd-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0a1bd-128">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="0a1bd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a1bd-129">Property</span></span>|<span data-ttu-id="0a1bd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a1bd-130">Type</span></span>|<span data-ttu-id="0a1bd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a1bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a1bd-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a1bd-132">roleScopeTagIds</span></span>|<span data-ttu-id="0a1bd-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1bd-133">String collection</span></span>|<span data-ttu-id="0a1bd-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0a1bd-135">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-135">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-136">id</span><span class="sxs-lookup"><span data-stu-id="0a1bd-136">id</span></span>|<span data-ttu-id="0a1bd-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1bd-137">String</span></span>|<span data-ttu-id="0a1bd-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-138">Key of the entity.</span></span> <span data-ttu-id="0a1bd-139">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-139">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1bd-140">createdDateTime</span></span>|<span data-ttu-id="0a1bd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1bd-141">DateTimeOffset</span></span>|<span data-ttu-id="0a1bd-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-142">DateTime the object was created.</span></span> <span data-ttu-id="0a1bd-143">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-143">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-144">descrição</span><span class="sxs-lookup"><span data-stu-id="0a1bd-144">description</span></span>|<span data-ttu-id="0a1bd-145">String</span><span class="sxs-lookup"><span data-stu-id="0a1bd-145">String</span></span>|<span data-ttu-id="0a1bd-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0a1bd-147">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-147">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a1bd-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0a1bd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a1bd-149">DateTimeOffset</span></span>|<span data-ttu-id="0a1bd-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-150">DateTime the object was last modified.</span></span> <span data-ttu-id="0a1bd-151">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-151">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-152">displayName</span><span class="sxs-lookup"><span data-stu-id="0a1bd-152">displayName</span></span>|<span data-ttu-id="0a1bd-153">String</span><span class="sxs-lookup"><span data-stu-id="0a1bd-153">String</span></span>|<span data-ttu-id="0a1bd-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0a1bd-155">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-155">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-156">version</span><span class="sxs-lookup"><span data-stu-id="0a1bd-156">version</span></span>|<span data-ttu-id="0a1bd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-157">Int32</span></span>|<span data-ttu-id="0a1bd-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-158">Version of the device configuration.</span></span> <span data-ttu-id="0a1bd-159">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a1bd-159">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0a1bd-160">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0a1bd-160">passwordRequired</span></span>|<span data-ttu-id="0a1bd-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a1bd-161">Boolean</span></span>|<span data-ttu-id="0a1bd-162">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-162">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="0a1bd-163">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0a1bd-163">passwordBlockSimple</span></span>|<span data-ttu-id="0a1bd-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a1bd-164">Boolean</span></span>|<span data-ttu-id="0a1bd-165">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-165">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="0a1bd-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0a1bd-166">passwordExpirationDays</span></span>|<span data-ttu-id="0a1bd-167">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-167">Int32</span></span>|<span data-ttu-id="0a1bd-168">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-168">Password expiration in days.</span></span>|
|<span data-ttu-id="0a1bd-169">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0a1bd-169">passwordMinimumLength</span></span>|<span data-ttu-id="0a1bd-170">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-170">Int32</span></span>|<span data-ttu-id="0a1bd-171">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-171">The minimum password length.</span></span>|
|<span data-ttu-id="0a1bd-172">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0a1bd-172">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0a1bd-173">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-173">Int32</span></span>|<span data-ttu-id="0a1bd-174">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-174">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0a1bd-175">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0a1bd-175">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0a1bd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-176">Int32</span></span>|<span data-ttu-id="0a1bd-177">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-177">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0a1bd-178">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0a1bd-178">passwordRequiredType</span></span>|[<span data-ttu-id="0a1bd-179">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0a1bd-179">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0a1bd-180">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-180">The required password type.</span></span> <span data-ttu-id="0a1bd-181">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-181">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0a1bd-182">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0a1bd-182">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0a1bd-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0a1bd-183">Int32</span></span>|<span data-ttu-id="0a1bd-184">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-184">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0a1bd-185">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="0a1bd-185">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0a1bd-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0a1bd-186">osMinimumVersion</span></span>|<span data-ttu-id="0a1bd-187">String</span><span class="sxs-lookup"><span data-stu-id="0a1bd-187">String</span></span>|<span data-ttu-id="0a1bd-188">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-188">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0a1bd-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0a1bd-189">osMaximumVersion</span></span>|<span data-ttu-id="0a1bd-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a1bd-190">String</span></span>|<span data-ttu-id="0a1bd-191">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-191">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0a1bd-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0a1bd-192">storageRequireEncryption</span></span>|<span data-ttu-id="0a1bd-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="0a1bd-193">Boolean</span></span>|<span data-ttu-id="0a1bd-194">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-194">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="0a1bd-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1bd-195">Response</span></span>
<span data-ttu-id="0a1bd-196">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-196">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a1bd-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a1bd-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a1bd-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a1bd-198">Request</span></span>
<span data-ttu-id="0a1bd-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a1bd-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a1bd-200">Response</span></span>
<span data-ttu-id="0a1bd-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a1bd-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




