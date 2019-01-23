---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 190bdcabd7662295c3c02a8fadac48d9ec966ba0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425572"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="d5c7f-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d5c7f-103">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="d5c7f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5c7f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5c7f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c7f-107">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d5c7f-107">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5c7f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5c7f-108">Prerequisites</span></span>
<span data-ttu-id="d5c7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d5c7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d5c7f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5c7f-111">Permission type</span></span>|<span data-ttu-id="d5c7f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c7f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c7f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5c7f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5c7f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c7f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-116">Not supported.</span></span>|
|<span data-ttu-id="d5c7f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5c7f-117">Application</span></span>|<span data-ttu-id="d5c7f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c7f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5c7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="d5c7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c7f-120">Request headers</span></span>
|<span data-ttu-id="d5c7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5c7f-121">Header</span></span>|<span data-ttu-id="d5c7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d5c7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5c7f-123">Authorization</span></span>|<span data-ttu-id="d5c7f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5c7f-125">Accept</span></span>|<span data-ttu-id="d5c7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c7f-127">Request body</span></span>
<span data-ttu-id="d5c7f-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d5c7f-128">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="d5c7f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d5c7f-129">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="d5c7f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5c7f-130">Property</span></span>|<span data-ttu-id="d5c7f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5c7f-131">Type</span></span>|<span data-ttu-id="d5c7f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5c7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5c7f-133">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5c7f-133">roleScopeTagIds</span></span>|<span data-ttu-id="d5c7f-134">String collection</span><span class="sxs-lookup"><span data-stu-id="d5c7f-134">String collection</span></span>|<span data-ttu-id="d5c7f-135">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-135">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5c7f-136">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-136">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-137">id</span><span class="sxs-lookup"><span data-stu-id="d5c7f-137">id</span></span>|<span data-ttu-id="d5c7f-138">String</span><span class="sxs-lookup"><span data-stu-id="d5c7f-138">String</span></span>|<span data-ttu-id="d5c7f-139">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-139">Key of the entity.</span></span> <span data-ttu-id="d5c7f-140">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-140">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5c7f-141">createdDateTime</span></span>|<span data-ttu-id="d5c7f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5c7f-142">DateTimeOffset</span></span>|<span data-ttu-id="d5c7f-143">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-143">DateTime the object was created.</span></span> <span data-ttu-id="d5c7f-144">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-144">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-145">description</span><span class="sxs-lookup"><span data-stu-id="d5c7f-145">description</span></span>|<span data-ttu-id="d5c7f-146">String</span><span class="sxs-lookup"><span data-stu-id="d5c7f-146">String</span></span>|<span data-ttu-id="d5c7f-147">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-147">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5c7f-148">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-148">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5c7f-149">lastModifiedDateTime</span></span>|<span data-ttu-id="d5c7f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5c7f-150">DateTimeOffset</span></span>|<span data-ttu-id="d5c7f-151">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-151">DateTime the object was last modified.</span></span> <span data-ttu-id="d5c7f-152">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-152">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d5c7f-153">displayName</span></span>|<span data-ttu-id="d5c7f-154">String</span><span class="sxs-lookup"><span data-stu-id="d5c7f-154">String</span></span>|<span data-ttu-id="d5c7f-155">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-155">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5c7f-156">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-156">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-157">version</span><span class="sxs-lookup"><span data-stu-id="d5c7f-157">version</span></span>|<span data-ttu-id="d5c7f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-158">Int32</span></span>|<span data-ttu-id="d5c7f-159">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-159">Version of the device configuration.</span></span> <span data-ttu-id="d5c7f-160">Herdado de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d5c7f-160">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d5c7f-161">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d5c7f-161">passwordBlockSimple</span></span>|<span data-ttu-id="d5c7f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5c7f-162">Boolean</span></span>|<span data-ttu-id="d5c7f-163">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-163">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="d5c7f-164">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d5c7f-164">passwordExpirationDays</span></span>|<span data-ttu-id="d5c7f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-165">Int32</span></span>|<span data-ttu-id="d5c7f-166">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-166">Number of days before the password expires.</span></span>|
|<span data-ttu-id="d5c7f-167">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d5c7f-167">passwordMinimumLength</span></span>|<span data-ttu-id="d5c7f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-168">Int32</span></span>|<span data-ttu-id="d5c7f-169">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-169">Minimum length of passwords.</span></span>|
|<span data-ttu-id="d5c7f-170">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d5c7f-170">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d5c7f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-171">Int32</span></span>|<span data-ttu-id="d5c7f-172">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-172">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d5c7f-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d5c7f-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d5c7f-174">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-174">Int32</span></span>|<span data-ttu-id="d5c7f-175">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-175">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d5c7f-176">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d5c7f-176">passwordRequiredType</span></span>|[<span data-ttu-id="d5c7f-177">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d5c7f-177">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d5c7f-178">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-178">The required password type.</span></span> <span data-ttu-id="d5c7f-179">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-179">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d5c7f-180">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d5c7f-180">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d5c7f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d5c7f-181">Int32</span></span>|<span data-ttu-id="d5c7f-182">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-182">Number of previous passwords to block.</span></span> <span data-ttu-id="d5c7f-183">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="d5c7f-183">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d5c7f-184">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d5c7f-184">passwordRequired</span></span>|<span data-ttu-id="d5c7f-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5c7f-185">Boolean</span></span>|<span data-ttu-id="d5c7f-186">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-186">Whether or not to require a password.</span></span>|
|<span data-ttu-id="d5c7f-187">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d5c7f-187">osMinimumVersion</span></span>|<span data-ttu-id="d5c7f-188">String</span><span class="sxs-lookup"><span data-stu-id="d5c7f-188">String</span></span>|<span data-ttu-id="d5c7f-189">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-189">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="d5c7f-190">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d5c7f-190">osMaximumVersion</span></span>|<span data-ttu-id="d5c7f-191">String</span><span class="sxs-lookup"><span data-stu-id="d5c7f-191">String</span></span>|<span data-ttu-id="d5c7f-192">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-192">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="d5c7f-193">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d5c7f-193">storageRequireEncryption</span></span>|<span data-ttu-id="d5c7f-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="d5c7f-194">Boolean</span></span>|<span data-ttu-id="d5c7f-195">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-195">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="d5c7f-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c7f-196">Response</span></span>
<span data-ttu-id="d5c7f-197">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-197">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c7f-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5c7f-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5c7f-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5c7f-199">Request</span></span>
<span data-ttu-id="d5c7f-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d5c7f-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5c7f-201">Response</span></span>
<span data-ttu-id="d5c7f-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5c7f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




