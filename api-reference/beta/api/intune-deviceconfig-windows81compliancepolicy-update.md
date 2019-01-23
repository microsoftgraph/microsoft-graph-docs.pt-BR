---
title: Atualizar windows81CompliancePolicy
description: Atualiza as propriedades de um objeto windows81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77b744aa62fddf7427496855a2e8a20239ff53ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413574"
---
# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="91d81-103">Atualizar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="91d81-103">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="91d81-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="91d81-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91d81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91d81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91d81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="91d81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91d81-107">Atualiza as propriedades de um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="91d81-107">Update the properties of a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91d81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91d81-108">Prerequisites</span></span>
<span data-ttu-id="91d81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="91d81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="91d81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91d81-111">Permission type</span></span>|<span data-ttu-id="91d81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91d81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91d81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91d81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91d81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91d81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91d81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91d81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91d81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d81-116">Not supported.</span></span>|
|<span data-ttu-id="91d81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91d81-117">Application</span></span>|<span data-ttu-id="91d81-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91d81-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91d81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91d81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="91d81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91d81-120">Request headers</span></span>
|<span data-ttu-id="91d81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91d81-121">Header</span></span>|<span data-ttu-id="91d81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="91d81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91d81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91d81-123">Authorization</span></span>|<span data-ttu-id="91d81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91d81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91d81-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91d81-125">Accept</span></span>|<span data-ttu-id="91d81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91d81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91d81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91d81-127">Request body</span></span>
<span data-ttu-id="91d81-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="91d81-128">In the request body, supply a JSON representation for the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="91d81-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="91d81-129">The following table shows the properties that are required when you create the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span></span>

|<span data-ttu-id="91d81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91d81-130">Property</span></span>|<span data-ttu-id="91d81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="91d81-131">Type</span></span>|<span data-ttu-id="91d81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="91d81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91d81-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91d81-133">roleScopeTagIds</span></span>|<span data-ttu-id="91d81-134">String collection</span><span class="sxs-lookup"><span data-stu-id="91d81-134">String collection</span></span>|<span data-ttu-id="91d81-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="91d81-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="91d81-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-137">id</span><span class="sxs-lookup"><span data-stu-id="91d81-137">id</span></span>|<span data-ttu-id="91d81-138">String</span><span class="sxs-lookup"><span data-stu-id="91d81-138">String</span></span>|<span data-ttu-id="91d81-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91d81-139">Key of the entity.</span></span> <span data-ttu-id="91d81-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91d81-141">createdDateTime</span></span>|<span data-ttu-id="91d81-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91d81-142">DateTimeOffset</span></span>|<span data-ttu-id="91d81-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="91d81-143">DateTime the object was created.</span></span> <span data-ttu-id="91d81-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-145">description</span><span class="sxs-lookup"><span data-stu-id="91d81-145">description</span></span>|<span data-ttu-id="91d81-146">String</span><span class="sxs-lookup"><span data-stu-id="91d81-146">String</span></span>|<span data-ttu-id="91d81-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91d81-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91d81-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91d81-149">lastModifiedDateTime</span></span>|<span data-ttu-id="91d81-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91d81-150">DateTimeOffset</span></span>|<span data-ttu-id="91d81-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="91d81-151">DateTime the object was last modified.</span></span> <span data-ttu-id="91d81-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-153">displayName</span><span class="sxs-lookup"><span data-stu-id="91d81-153">displayName</span></span>|<span data-ttu-id="91d81-154">String</span><span class="sxs-lookup"><span data-stu-id="91d81-154">String</span></span>|<span data-ttu-id="91d81-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91d81-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91d81-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-157">version</span><span class="sxs-lookup"><span data-stu-id="91d81-157">version</span></span>|<span data-ttu-id="91d81-158">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-158">Int32</span></span>|<span data-ttu-id="91d81-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91d81-159">Version of the device configuration.</span></span> <span data-ttu-id="91d81-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="91d81-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="91d81-161">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="91d81-161">passwordRequired</span></span>|<span data-ttu-id="91d81-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="91d81-162">Boolean</span></span>|<span data-ttu-id="91d81-163">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="91d81-163">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="91d81-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="91d81-164">passwordBlockSimple</span></span>|<span data-ttu-id="91d81-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="91d81-165">Boolean</span></span>|<span data-ttu-id="91d81-166">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="91d81-166">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="91d81-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="91d81-167">passwordExpirationDays</span></span>|<span data-ttu-id="91d81-168">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-168">Int32</span></span>|<span data-ttu-id="91d81-169">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="91d81-169">Password expiration in days.</span></span>|
|<span data-ttu-id="91d81-170">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="91d81-170">passwordMinimumLength</span></span>|<span data-ttu-id="91d81-171">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-171">Int32</span></span>|<span data-ttu-id="91d81-172">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="91d81-172">The minimum password length.</span></span>|
|<span data-ttu-id="91d81-173">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="91d81-173">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="91d81-174">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-174">Int32</span></span>|<span data-ttu-id="91d81-175">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="91d81-175">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="91d81-176">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="91d81-176">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="91d81-177">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-177">Int32</span></span>|<span data-ttu-id="91d81-178">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="91d81-178">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="91d81-179">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="91d81-179">passwordRequiredType</span></span>|[<span data-ttu-id="91d81-180">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="91d81-180">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="91d81-181">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="91d81-181">The required password type.</span></span> <span data-ttu-id="91d81-182">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="91d81-182">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="91d81-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="91d81-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="91d81-184">Int32</span><span class="sxs-lookup"><span data-stu-id="91d81-184">Int32</span></span>|<span data-ttu-id="91d81-185">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="91d81-185">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="91d81-186">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="91d81-186">Valid values 0 to 24</span></span>|
|<span data-ttu-id="91d81-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="91d81-187">osMinimumVersion</span></span>|<span data-ttu-id="91d81-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91d81-188">String</span></span>|<span data-ttu-id="91d81-189">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="91d81-189">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="91d81-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="91d81-190">osMaximumVersion</span></span>|<span data-ttu-id="91d81-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91d81-191">String</span></span>|<span data-ttu-id="91d81-192">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="91d81-192">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="91d81-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="91d81-193">storageRequireEncryption</span></span>|<span data-ttu-id="91d81-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="91d81-194">Boolean</span></span>|<span data-ttu-id="91d81-195">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="91d81-195">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="91d81-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d81-196">Response</span></span>
<span data-ttu-id="91d81-197">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91d81-197">If successful, this method returns a `200 OK` response code and an updated [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91d81-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91d81-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="91d81-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91d81-199">Request</span></span>
<span data-ttu-id="91d81-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91d81-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91d81-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="91d81-201">Response</span></span>
<span data-ttu-id="91d81-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91d81-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




