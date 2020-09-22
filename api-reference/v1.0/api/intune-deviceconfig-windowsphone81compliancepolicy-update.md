---
title: Atualizar windowsPhone81CompliancePolicy
description: Atualizar as propriedades de um objeto windowsPhone81CompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83a938e8ec8eb99ef99f535b56799ab542d80830
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069810"
---
# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="f9509-103">Atualizar windowsPhone81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f9509-103">Update windowsPhone81CompliancePolicy</span></span>

<span data-ttu-id="f9509-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9509-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9509-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9509-106">Atualizar as propriedades de um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f9509-106">Update the properties of a [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9509-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9509-107">Prerequisites</span></span>
<span data-ttu-id="f9509-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9509-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9509-110">Permission type</span></span>|<span data-ttu-id="f9509-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9509-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9509-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9509-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9509-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9509-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9509-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9509-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9509-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9509-115">Not supported.</span></span>|
|<span data-ttu-id="f9509-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9509-116">Application</span></span>|<span data-ttu-id="f9509-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9509-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9509-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9509-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="f9509-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9509-119">Request headers</span></span>
|<span data-ttu-id="f9509-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9509-120">Header</span></span>|<span data-ttu-id="f9509-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f9509-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9509-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9509-122">Authorization</span></span>|<span data-ttu-id="f9509-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9509-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9509-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9509-124">Accept</span></span>|<span data-ttu-id="f9509-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9509-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9509-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9509-126">Request body</span></span>
<span data-ttu-id="f9509-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f9509-127">In the request body, supply a JSON representation for the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="f9509-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f9509-128">The following table shows the properties that are required when you create the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md).</span></span>

|<span data-ttu-id="f9509-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9509-129">Property</span></span>|<span data-ttu-id="f9509-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9509-130">Type</span></span>|<span data-ttu-id="f9509-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9509-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9509-132">id</span><span class="sxs-lookup"><span data-stu-id="f9509-132">id</span></span>|<span data-ttu-id="f9509-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9509-133">String</span></span>|<span data-ttu-id="f9509-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9509-134">Key of the entity.</span></span> <span data-ttu-id="f9509-135">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-135">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9509-136">createdDateTime</span></span>|<span data-ttu-id="f9509-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9509-137">DateTimeOffset</span></span>|<span data-ttu-id="f9509-138">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9509-138">DateTime the object was created.</span></span> <span data-ttu-id="f9509-139">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-139">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-140">description</span><span class="sxs-lookup"><span data-stu-id="f9509-140">description</span></span>|<span data-ttu-id="f9509-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9509-141">String</span></span>|<span data-ttu-id="f9509-142">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9509-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9509-143">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-143">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9509-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f9509-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9509-145">DateTimeOffset</span></span>|<span data-ttu-id="f9509-146">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9509-146">DateTime the object was last modified.</span></span> <span data-ttu-id="f9509-147">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-147">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f9509-148">displayName</span></span>|<span data-ttu-id="f9509-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9509-149">String</span></span>|<span data-ttu-id="f9509-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9509-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9509-151">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-151">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-152">version</span><span class="sxs-lookup"><span data-stu-id="f9509-152">version</span></span>|<span data-ttu-id="f9509-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-153">Int32</span></span>|<span data-ttu-id="f9509-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9509-154">Version of the device configuration.</span></span> <span data-ttu-id="f9509-155">Herdada de [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f9509-155">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="f9509-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f9509-156">passwordBlockSimple</span></span>|<span data-ttu-id="f9509-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9509-157">Boolean</span></span>|<span data-ttu-id="f9509-158">Se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f9509-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="f9509-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f9509-159">passwordExpirationDays</span></span>|<span data-ttu-id="f9509-160">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-160">Int32</span></span>|<span data-ttu-id="f9509-161">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f9509-161">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f9509-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f9509-162">passwordMinimumLength</span></span>|<span data-ttu-id="f9509-163">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-163">Int32</span></span>|<span data-ttu-id="f9509-164">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f9509-164">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f9509-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f9509-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f9509-166">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-166">Int32</span></span>|<span data-ttu-id="f9509-167">Minutos de inatividade antes que uma senha seja necessária.</span><span class="sxs-lookup"><span data-stu-id="f9509-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="f9509-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f9509-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f9509-169">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-169">Int32</span></span>|<span data-ttu-id="f9509-170">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="f9509-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="f9509-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f9509-171">passwordRequiredType</span></span>|[<span data-ttu-id="f9509-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f9509-172">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f9509-173">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="f9509-173">The required password type.</span></span> <span data-ttu-id="f9509-174">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f9509-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f9509-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f9509-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f9509-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f9509-176">Int32</span></span>|<span data-ttu-id="f9509-177">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f9509-177">Number of previous passwords to block.</span></span> <span data-ttu-id="f9509-178">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f9509-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f9509-179">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f9509-179">passwordRequired</span></span>|<span data-ttu-id="f9509-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9509-180">Boolean</span></span>|<span data-ttu-id="f9509-181">Se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="f9509-181">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f9509-182">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f9509-182">osMinimumVersion</span></span>|<span data-ttu-id="f9509-183">String</span><span class="sxs-lookup"><span data-stu-id="f9509-183">String</span></span>|<span data-ttu-id="f9509-184">Versão mínima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f9509-184">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="f9509-185">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f9509-185">osMaximumVersion</span></span>|<span data-ttu-id="f9509-186">String</span><span class="sxs-lookup"><span data-stu-id="f9509-186">String</span></span>|<span data-ttu-id="f9509-187">Versão máxima do Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f9509-187">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="f9509-188">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="f9509-188">storageRequireEncryption</span></span>|<span data-ttu-id="f9509-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9509-189">Boolean</span></span>|<span data-ttu-id="f9509-190">Exige criptografia em dispositivos Windows Phone.</span><span class="sxs-lookup"><span data-stu-id="f9509-190">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="f9509-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9509-191">Response</span></span>
<span data-ttu-id="f9509-192">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9509-192">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9509-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9509-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9509-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9509-194">Request</span></span>
<span data-ttu-id="f9509-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9509-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="f9509-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9509-196">Response</span></span>
<span data-ttu-id="f9509-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9509-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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









