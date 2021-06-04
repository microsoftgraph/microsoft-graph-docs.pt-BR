---
title: Criar windows81CompliancePolicy
description: Cria um novo objeto windows81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b5cc71fa9e35021afae933079a76ea257328b37a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752655"
---
# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="6a268-103">Criar windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="6a268-103">Create windows81CompliancePolicy</span></span>

<span data-ttu-id="6a268-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a268-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a268-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a268-106">Cria um novo objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6a268-106">Create a new [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a268-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a268-107">Prerequisites</span></span>
<span data-ttu-id="6a268-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a268-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a268-110">Permission type</span></span>|<span data-ttu-id="6a268-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a268-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a268-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a268-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a268-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a268-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a268-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a268-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a268-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a268-115">Not supported.</span></span>|
|<span data-ttu-id="6a268-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a268-116">Application</span></span>|<span data-ttu-id="6a268-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a268-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a268-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a268-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6a268-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a268-119">Request headers</span></span>
|<span data-ttu-id="6a268-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a268-120">Header</span></span>|<span data-ttu-id="6a268-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a268-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a268-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a268-122">Authorization</span></span>|<span data-ttu-id="6a268-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a268-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a268-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a268-124">Accept</span></span>|<span data-ttu-id="6a268-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a268-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a268-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a268-126">Request body</span></span>
<span data-ttu-id="6a268-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="6a268-127">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="6a268-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81CompliancePolicy.</span><span class="sxs-lookup"><span data-stu-id="6a268-128">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="6a268-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a268-129">Property</span></span>|<span data-ttu-id="6a268-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a268-130">Type</span></span>|<span data-ttu-id="6a268-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a268-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a268-132">id</span><span class="sxs-lookup"><span data-stu-id="6a268-132">id</span></span>|<span data-ttu-id="6a268-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a268-133">String</span></span>|<span data-ttu-id="6a268-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a268-134">Key of the entity.</span></span> <span data-ttu-id="6a268-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a268-136">createdDateTime</span></span>|<span data-ttu-id="6a268-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a268-137">DateTimeOffset</span></span>|<span data-ttu-id="6a268-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6a268-138">DateTime the object was created.</span></span> <span data-ttu-id="6a268-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-140">descrição</span><span class="sxs-lookup"><span data-stu-id="6a268-140">description</span></span>|<span data-ttu-id="6a268-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a268-141">String</span></span>|<span data-ttu-id="6a268-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a268-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a268-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a268-144">lastModifiedDateTime</span></span>|<span data-ttu-id="6a268-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a268-145">DateTimeOffset</span></span>|<span data-ttu-id="6a268-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6a268-146">DateTime the object was last modified.</span></span> <span data-ttu-id="6a268-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-148">displayName</span><span class="sxs-lookup"><span data-stu-id="6a268-148">displayName</span></span>|<span data-ttu-id="6a268-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a268-149">String</span></span>|<span data-ttu-id="6a268-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a268-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a268-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-152">version</span><span class="sxs-lookup"><span data-stu-id="6a268-152">version</span></span>|<span data-ttu-id="6a268-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-153">Int32</span></span>|<span data-ttu-id="6a268-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a268-154">Version of the device configuration.</span></span> <span data-ttu-id="6a268-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a268-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6a268-156">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6a268-156">passwordRequired</span></span>|<span data-ttu-id="6a268-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a268-157">Boolean</span></span>|<span data-ttu-id="6a268-158">Exige uma senha para desbloquear o dispositivo Windows.</span><span class="sxs-lookup"><span data-stu-id="6a268-158">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="6a268-159">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6a268-159">passwordBlockSimple</span></span>|<span data-ttu-id="6a268-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a268-160">Boolean</span></span>|<span data-ttu-id="6a268-161">Indica se a senha simples deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6a268-161">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="6a268-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6a268-162">passwordExpirationDays</span></span>|<span data-ttu-id="6a268-163">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-163">Int32</span></span>|<span data-ttu-id="6a268-164">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="6a268-164">Password expiration in days.</span></span>|
|<span data-ttu-id="6a268-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6a268-165">passwordMinimumLength</span></span>|<span data-ttu-id="6a268-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-166">Int32</span></span>|<span data-ttu-id="6a268-167">Comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="6a268-167">The minimum password length.</span></span>|
|<span data-ttu-id="6a268-168">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6a268-168">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6a268-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-169">Int32</span></span>|<span data-ttu-id="6a268-170">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6a268-170">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6a268-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6a268-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6a268-172">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-172">Int32</span></span>|<span data-ttu-id="6a268-173">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="6a268-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6a268-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6a268-174">passwordRequiredType</span></span>|[<span data-ttu-id="6a268-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6a268-175">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6a268-176">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="6a268-176">The required password type.</span></span> <span data-ttu-id="6a268-177">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6a268-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6a268-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6a268-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6a268-179">Int32</span><span class="sxs-lookup"><span data-stu-id="6a268-179">Int32</span></span>|<span data-ttu-id="6a268-180">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="6a268-180">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="6a268-181">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="6a268-181">Valid values 0 to 24</span></span>|
|<span data-ttu-id="6a268-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6a268-182">osMinimumVersion</span></span>|<span data-ttu-id="6a268-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a268-183">String</span></span>|<span data-ttu-id="6a268-184">Versão mínima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="6a268-184">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="6a268-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6a268-185">osMaximumVersion</span></span>|<span data-ttu-id="6a268-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a268-186">String</span></span>|<span data-ttu-id="6a268-187">Versão máxima do Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="6a268-187">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="6a268-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6a268-188">storageRequireEncryption</span></span>|<span data-ttu-id="6a268-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a268-189">Boolean</span></span>|<span data-ttu-id="6a268-190">Indica se a criptografia é ou não necessária em um dispositivo Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="6a268-190">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="6a268-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a268-191">Response</span></span>
<span data-ttu-id="6a268-192">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a268-192">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a268-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a268-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a268-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a268-194">Request</span></span>
<span data-ttu-id="6a268-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a268-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
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

### <a name="response"></a><span data-ttu-id="6a268-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a268-196">Response</span></span>
<span data-ttu-id="6a268-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a268-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




