---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b2b9d1fb0e661e16d8ae377a8674cfe1bbc482b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147667"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="aa67c-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="aa67c-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="aa67c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa67c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa67c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa67c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa67c-106">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa67c-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa67c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa67c-107">Prerequisites</span></span>
<span data-ttu-id="aa67c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa67c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aa67c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa67c-110">Permission type</span></span>|<span data-ttu-id="aa67c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa67c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa67c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa67c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa67c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa67c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa67c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa67c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa67c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa67c-115">Not supported.</span></span>|
|<span data-ttu-id="aa67c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa67c-116">Application</span></span>|<span data-ttu-id="aa67c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa67c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa67c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa67c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="aa67c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa67c-119">Request headers</span></span>
|<span data-ttu-id="aa67c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa67c-120">Header</span></span>|<span data-ttu-id="aa67c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa67c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa67c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa67c-122">Authorization</span></span>|<span data-ttu-id="aa67c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa67c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa67c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa67c-124">Accept</span></span>|<span data-ttu-id="aa67c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa67c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa67c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa67c-126">Request body</span></span>
<span data-ttu-id="aa67c-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa67c-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="aa67c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="aa67c-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="aa67c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa67c-129">Property</span></span>|<span data-ttu-id="aa67c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa67c-130">Type</span></span>|<span data-ttu-id="aa67c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa67c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa67c-132">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa67c-132">roleScopeTagIds</span></span>|<span data-ttu-id="aa67c-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa67c-133">String collection</span></span>|<span data-ttu-id="aa67c-134">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aa67c-134">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa67c-135">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-136">id</span><span class="sxs-lookup"><span data-stu-id="aa67c-136">id</span></span>|<span data-ttu-id="aa67c-137">String</span><span class="sxs-lookup"><span data-stu-id="aa67c-137">String</span></span>|<span data-ttu-id="aa67c-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa67c-138">Key of the entity.</span></span> <span data-ttu-id="aa67c-139">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa67c-140">createdDateTime</span></span>|<span data-ttu-id="aa67c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa67c-141">DateTimeOffset</span></span>|<span data-ttu-id="aa67c-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aa67c-142">DateTime the object was created.</span></span> <span data-ttu-id="aa67c-143">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-144">description</span><span class="sxs-lookup"><span data-stu-id="aa67c-144">description</span></span>|<span data-ttu-id="aa67c-145">String</span><span class="sxs-lookup"><span data-stu-id="aa67c-145">String</span></span>|<span data-ttu-id="aa67c-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa67c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa67c-147">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa67c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="aa67c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa67c-149">DateTimeOffset</span></span>|<span data-ttu-id="aa67c-150">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aa67c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="aa67c-151">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="aa67c-152">displayName</span></span>|<span data-ttu-id="aa67c-153">String</span><span class="sxs-lookup"><span data-stu-id="aa67c-153">String</span></span>|<span data-ttu-id="aa67c-154">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa67c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa67c-155">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-156">version</span><span class="sxs-lookup"><span data-stu-id="aa67c-156">version</span></span>|<span data-ttu-id="aa67c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-157">Int32</span></span>|<span data-ttu-id="aa67c-158">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa67c-158">Version of the device configuration.</span></span> <span data-ttu-id="aa67c-159">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="aa67c-159">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="aa67c-160">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="aa67c-160">passwordBlockSimple</span></span>|<span data-ttu-id="aa67c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa67c-161">Boolean</span></span>|<span data-ttu-id="aa67c-162">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="aa67c-162">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="aa67c-163">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="aa67c-163">passwordExpirationDays</span></span>|<span data-ttu-id="aa67c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-164">Int32</span></span>|<span data-ttu-id="aa67c-165">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="aa67c-165">Number of days before the password expires.</span></span>|
|<span data-ttu-id="aa67c-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="aa67c-166">passwordMinimumLength</span></span>|<span data-ttu-id="aa67c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-167">Int32</span></span>|<span data-ttu-id="aa67c-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="aa67c-168">Minimum length of passwords.</span></span>|
|<span data-ttu-id="aa67c-169">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="aa67c-169">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="aa67c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-170">Int32</span></span>|<span data-ttu-id="aa67c-171">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="aa67c-171">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="aa67c-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="aa67c-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="aa67c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-173">Int32</span></span>|<span data-ttu-id="aa67c-174">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="aa67c-174">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="aa67c-175">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="aa67c-175">passwordRequiredType</span></span>|[<span data-ttu-id="aa67c-176">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="aa67c-176">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="aa67c-177">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="aa67c-177">The required password type.</span></span> <span data-ttu-id="aa67c-178">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="aa67c-178">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="aa67c-179">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="aa67c-179">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="aa67c-180">Int32</span><span class="sxs-lookup"><span data-stu-id="aa67c-180">Int32</span></span>|<span data-ttu-id="aa67c-181">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="aa67c-181">Number of previous passwords to block.</span></span> <span data-ttu-id="aa67c-182">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="aa67c-182">Valid values 0 to 24</span></span>|
|<span data-ttu-id="aa67c-183">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="aa67c-183">passwordRequired</span></span>|<span data-ttu-id="aa67c-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa67c-184">Boolean</span></span>|<span data-ttu-id="aa67c-185">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="aa67c-185">Whether or not to require a password.</span></span>|
|<span data-ttu-id="aa67c-186">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="aa67c-186">osMinimumVersion</span></span>|<span data-ttu-id="aa67c-187">String</span><span class="sxs-lookup"><span data-stu-id="aa67c-187">String</span></span>|<span data-ttu-id="aa67c-188">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aa67c-188">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="aa67c-189">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="aa67c-189">osMaximumVersion</span></span>|<span data-ttu-id="aa67c-190">String</span><span class="sxs-lookup"><span data-stu-id="aa67c-190">String</span></span>|<span data-ttu-id="aa67c-191">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aa67c-191">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="aa67c-192">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="aa67c-192">storageRequireEncryption</span></span>|<span data-ttu-id="aa67c-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa67c-193">Boolean</span></span>|<span data-ttu-id="aa67c-194">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="aa67c-194">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="aa67c-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa67c-195">Response</span></span>
<span data-ttu-id="aa67c-196">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa67c-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa67c-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa67c-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa67c-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa67c-198">Request</span></span>
<span data-ttu-id="aa67c-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa67c-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa67c-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa67c-200">Response</span></span>
<span data-ttu-id="aa67c-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa67c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




