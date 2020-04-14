---
title: Criar windows81CompliancePolicy
description: Cria um novo objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c135dd7951cd36639072bc98b0dcc2b3947e7fff
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43337372"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="2944a-103">Criar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2944a-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="2944a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2944a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2944a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2944a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2944a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2944a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2944a-107">Cria um novo objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2944a-107">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2944a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2944a-108">Prerequisites</span></span>
<span data-ttu-id="2944a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2944a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2944a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2944a-111">Permission type</span></span>|<span data-ttu-id="2944a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2944a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2944a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2944a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2944a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2944a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2944a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2944a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2944a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2944a-116">Not supported.</span></span>|
|<span data-ttu-id="2944a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2944a-117">Application</span></span>|<span data-ttu-id="2944a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2944a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2944a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2944a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="2944a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2944a-120">Request headers</span></span>
|<span data-ttu-id="2944a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2944a-121">Header</span></span>|<span data-ttu-id="2944a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2944a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2944a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2944a-123">Authorization</span></span>|<span data-ttu-id="2944a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2944a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2944a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2944a-125">Accept</span></span>|<span data-ttu-id="2944a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2944a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2944a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2944a-127">Request body</span></span>
<span data-ttu-id="2944a-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2944a-128">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="2944a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="2944a-129">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="2944a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2944a-130">Property</span></span>|<span data-ttu-id="2944a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2944a-131">Type</span></span>|<span data-ttu-id="2944a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2944a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2944a-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2944a-133">roleScopeTagIds</span></span>|<span data-ttu-id="2944a-134">Coleção String</span><span class="sxs-lookup"><span data-stu-id="2944a-134">String collection</span></span>|<span data-ttu-id="2944a-135">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2944a-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2944a-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-137">id</span><span class="sxs-lookup"><span data-stu-id="2944a-137">id</span></span>|<span data-ttu-id="2944a-138">String</span><span class="sxs-lookup"><span data-stu-id="2944a-138">String</span></span>|<span data-ttu-id="2944a-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2944a-139">Key of the entity.</span></span> <span data-ttu-id="2944a-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2944a-141">createdDateTime</span></span>|<span data-ttu-id="2944a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2944a-142">DateTimeOffset</span></span>|<span data-ttu-id="2944a-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2944a-143">DateTime the object was created.</span></span> <span data-ttu-id="2944a-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-145">description</span><span class="sxs-lookup"><span data-stu-id="2944a-145">description</span></span>|<span data-ttu-id="2944a-146">String</span><span class="sxs-lookup"><span data-stu-id="2944a-146">String</span></span>|<span data-ttu-id="2944a-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2944a-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2944a-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2944a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2944a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2944a-150">DateTimeOffset</span></span>|<span data-ttu-id="2944a-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2944a-151">DateTime the object was last modified.</span></span> <span data-ttu-id="2944a-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2944a-153">displayName</span></span>|<span data-ttu-id="2944a-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2944a-154">String</span></span>|<span data-ttu-id="2944a-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2944a-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2944a-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-157">version</span><span class="sxs-lookup"><span data-stu-id="2944a-157">version</span></span>|<span data-ttu-id="2944a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-158">Int32</span></span>|<span data-ttu-id="2944a-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2944a-159">Version of the device configuration.</span></span> <span data-ttu-id="2944a-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2944a-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="2944a-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="2944a-161">passwordRequired</span></span>|<span data-ttu-id="2944a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2944a-162">Boolean</span></span>|<span data-ttu-id="2944a-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="2944a-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="2944a-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="2944a-164">passwordBlockSimple</span></span>|<span data-ttu-id="2944a-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="2944a-165">Boolean</span></span>|<span data-ttu-id="2944a-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="2944a-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="2944a-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2944a-167">passwordExpirationDays</span></span>|<span data-ttu-id="2944a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-168">Int32</span></span>|<span data-ttu-id="2944a-169">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="2944a-169">Password expiration in days.</span></span>|
|<span data-ttu-id="2944a-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2944a-170">passwordMinimumLength</span></span>|<span data-ttu-id="2944a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-171">Int32</span></span>|<span data-ttu-id="2944a-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="2944a-172">The minimum password length.</span></span>|
|<span data-ttu-id="2944a-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="2944a-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="2944a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-174">Int32</span></span>|<span data-ttu-id="2944a-175">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="2944a-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="2944a-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="2944a-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="2944a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-177">Int32</span></span>|<span data-ttu-id="2944a-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="2944a-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="2944a-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2944a-179">passwordRequiredType</span></span>|[<span data-ttu-id="2944a-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2944a-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="2944a-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="2944a-181">The required password type.</span></span> <span data-ttu-id="2944a-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="2944a-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="2944a-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2944a-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2944a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2944a-184">Int32</span></span>|<span data-ttu-id="2944a-185">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="2944a-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="2944a-186">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="2944a-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2944a-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2944a-187">osMinimumVersion</span></span>|<span data-ttu-id="2944a-188">String</span><span class="sxs-lookup"><span data-stu-id="2944a-188">String</span></span>|<span data-ttu-id="2944a-189">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="2944a-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="2944a-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2944a-190">osMaximumVersion</span></span>|<span data-ttu-id="2944a-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2944a-191">String</span></span>|<span data-ttu-id="2944a-192">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="2944a-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="2944a-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="2944a-193">storageRequireEncryption</span></span>|<span data-ttu-id="2944a-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="2944a-194">Boolean</span></span>|<span data-ttu-id="2944a-195">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="2944a-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="2944a-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="2944a-196">Response</span></span>
<span data-ttu-id="2944a-197">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2944a-197">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2944a-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2944a-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="2944a-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2944a-199">Request</span></span>
<span data-ttu-id="2944a-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2944a-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="2944a-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="2944a-201">Response</span></span>
<span data-ttu-id="2944a-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2944a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



