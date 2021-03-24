---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f49e5c39e525925a622fc8030773bd93a9fbaee
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132258"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="b6bb1-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b6bb1-103">Update windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="b6bb1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6bb1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6bb1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6bb1-107">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6bb1-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6bb1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6bb1-108">Prerequisites</span></span>
<span data-ttu-id="b6bb1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6bb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6bb1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6bb1-111">Permission type</span></span>|<span data-ttu-id="b6bb1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6bb1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6bb1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bb1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6bb1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6bb1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-116">Not supported.</span></span>|
|<span data-ttu-id="b6bb1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6bb1-117">Application</span></span>|<span data-ttu-id="b6bb1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6bb1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6bb1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6bb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b6bb1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bb1-120">Request headers</span></span>
|<span data-ttu-id="b6bb1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6bb1-121">Header</span></span>|<span data-ttu-id="b6bb1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6bb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6bb1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6bb1-123">Authorization</span></span>|<span data-ttu-id="b6bb1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6bb1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6bb1-125">Accept</span></span>|<span data-ttu-id="b6bb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6bb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6bb1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bb1-127">Request body</span></span>
<span data-ttu-id="b6bb1-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6bb1-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="b6bb1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6bb1-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="b6bb1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6bb1-130">Property</span></span>|<span data-ttu-id="b6bb1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6bb1-131">Type</span></span>|<span data-ttu-id="b6bb1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6bb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6bb1-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6bb1-133">roleScopeTagIds</span></span>|<span data-ttu-id="b6bb1-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6bb1-134">String collection</span></span>|<span data-ttu-id="b6bb1-135">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6bb1-136">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-136">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-137">id</span><span class="sxs-lookup"><span data-stu-id="b6bb1-137">id</span></span>|<span data-ttu-id="b6bb1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6bb1-138">String</span></span>|<span data-ttu-id="b6bb1-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-139">Key of the entity.</span></span> <span data-ttu-id="b6bb1-140">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-140">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bb1-141">createdDateTime</span></span>|<span data-ttu-id="b6bb1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bb1-142">DateTimeOffset</span></span>|<span data-ttu-id="b6bb1-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-143">DateTime the object was created.</span></span> <span data-ttu-id="b6bb1-144">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-144">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-145">descrição</span><span class="sxs-lookup"><span data-stu-id="b6bb1-145">description</span></span>|<span data-ttu-id="b6bb1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6bb1-146">String</span></span>|<span data-ttu-id="b6bb1-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6bb1-148">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-148">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bb1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="b6bb1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bb1-150">DateTimeOffset</span></span>|<span data-ttu-id="b6bb1-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-151">DateTime the object was last modified.</span></span> <span data-ttu-id="b6bb1-152">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-152">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-153">displayName</span><span class="sxs-lookup"><span data-stu-id="b6bb1-153">displayName</span></span>|<span data-ttu-id="b6bb1-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6bb1-154">String</span></span>|<span data-ttu-id="b6bb1-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6bb1-156">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-156">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-157">version</span><span class="sxs-lookup"><span data-stu-id="b6bb1-157">version</span></span>|<span data-ttu-id="b6bb1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-158">Int32</span></span>|<span data-ttu-id="b6bb1-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-159">Version of the device configuration.</span></span> <span data-ttu-id="b6bb1-160">Herdada de [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b6bb1-160">Inherited from [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6bb1-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b6bb1-161">passwordBlockSimple</span></span>|<span data-ttu-id="b6bb1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6bb1-162">Boolean</span></span>|<span data-ttu-id="b6bb1-163">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="b6bb1-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6bb1-164">passwordExpirationDays</span></span>|<span data-ttu-id="b6bb1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-165">Int32</span></span>|<span data-ttu-id="b6bb1-166">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="b6bb1-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6bb1-167">passwordMinimumLength</span></span>|<span data-ttu-id="b6bb1-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-168">Int32</span></span>|<span data-ttu-id="b6bb1-169">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="b6bb1-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6bb1-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6bb1-171">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-171">Int32</span></span>|<span data-ttu-id="b6bb1-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6bb1-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b6bb1-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b6bb1-174">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-174">Int32</span></span>|<span data-ttu-id="b6bb1-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b6bb1-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6bb1-176">passwordRequiredType</span></span>|[<span data-ttu-id="b6bb1-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b6bb1-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b6bb1-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-178">The required password type.</span></span> <span data-ttu-id="b6bb1-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b6bb1-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6bb1-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b6bb1-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b6bb1-181">Int32</span></span>|<span data-ttu-id="b6bb1-182">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-182">Number of previous passwords to block.</span></span> <span data-ttu-id="b6bb1-183">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b6bb1-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b6bb1-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6bb1-184">passwordRequired</span></span>|<span data-ttu-id="b6bb1-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6bb1-185">Boolean</span></span>|<span data-ttu-id="b6bb1-186">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b6bb1-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6bb1-187">osMinimumVersion</span></span>|<span data-ttu-id="b6bb1-188">String</span><span class="sxs-lookup"><span data-stu-id="b6bb1-188">String</span></span>|<span data-ttu-id="b6bb1-189">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="b6bb1-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6bb1-190">osMaximumVersion</span></span>|<span data-ttu-id="b6bb1-191">String</span><span class="sxs-lookup"><span data-stu-id="b6bb1-191">String</span></span>|<span data-ttu-id="b6bb1-192">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="b6bb1-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6bb1-193">storageRequireEncryption</span></span>|<span data-ttu-id="b6bb1-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6bb1-194">Boolean</span></span>|<span data-ttu-id="b6bb1-195">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="b6bb1-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bb1-196">Response</span></span>
<span data-ttu-id="b6bb1-197">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6bb1-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6bb1-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6bb1-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6bb1-199">Request</span></span>
<span data-ttu-id="b6bb1-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 669

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="b6bb1-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6bb1-201">Response</span></span>
<span data-ttu-id="b6bb1-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6bb1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```




